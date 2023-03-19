---
{"dg-publish":true,"permalink":"/branch-prediction/","tags":["datorteknik"]}
---

Man gissar vilken instruktion nästa ska vara, dvs om det ska ske ett hopp eller inte. Om man gissar rätt får man en mindre penalty än om man gissar fel.

Vid **Speculative Execution** fortsätter man att exekvera en instruktion, utifall att det är rätt. Om man har gissat rätt får man ingen penalty alls! Om man gissar fel blir penaltyn lika stor som om man inte använde speculative execution. En bra prediktering är alltså oerhört viktigt.

# Static Branch Prediction
Ingen hänsyn tas till exekveringshistoriken. 
Exempelvis
- Predict never taken - anta att hoppet inte kommer tas
- Predict always taken - antar att hoppet alltid kommer tas
- Predict beroende på riktnig

# Dynamisk Branch Prediction
Exekveringshistoriken tas i hänsyn. Man kan använda en bit för prediktion, där utfallet från förra gången hoppinstruktionen används och man gissar att samma sak ska hända som förra gången. 

Detta kan utvecklas genom tvåbitars prediktering, där man har två bitar istället för en. Om man gissat fel två gånger ändrar man gissning.
![Pasted image 20230131164747.png](/img/user/images/Pasted%20image%2020230131164747.png)

