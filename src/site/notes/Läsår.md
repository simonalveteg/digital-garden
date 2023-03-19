```dataviewjs
let pages = dv.pages("#course AND #moc");
for (let group of pages.groupBy(b => b.study_year)) { 
	dv.header(1, "Year "+group.key);
	dv.table(
		["Course","Code","LP","HP"],
		group.rows.sort(b => b.study_period).map(b => [b.file.link,b.course_code,b.study_period,b.hp])
	);
}
```