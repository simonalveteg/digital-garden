```dataviewjs
let course = "datorteknik";
let tags = new Map();
tags.set("Föreläsning","Föreläsningar");
tags.set("Laboration","Laborationer");
tags.set("Övning","Övningar");
tags.set("Seminarium","Seminarium");
tags.set("Inlämning","Inlämningar");
for (let [key,value] of tags) {
	let pages = dv.pages("#"+key+" and #"+course);
	if (pages.length > 0) {
		dv.header(1, value);
		dv.table(["File","Modified","Links"], pages
			.sort(b => -b.file.mtime)
			.map(b => [b.file.link, b.file.mtime, b.file.outlinks.length])
		);
	}
}
dv.header(1, "Alla anteckningar");
dv.table(["File","Modified","Links"], dv.pages("#"+course)
	.sort(b => -b.file.mtime)
	.map(b => [b.file.link, b.file.mtime, b.file.outlinks.length])
);
```