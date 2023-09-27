---
title: "Qualitative data cleaning"
authors: "Xu Chu, Ihab F. Ilyas"
year: 2016
---

Keywords: #DataCleaning #DataPreparation #AutomaticEDA #EDA #QualitativeData 

### Notes

Error classification taxonomy:
	Data can be subject to Integrity constraints; functional dependencies, denial constraints

It is time consuming to design ICs and needs expert knowledge

Error detection is constrained by a lack of expressiveness in how we describe the constraints and quality rules on data

Two phases: Error detection & Error Repairing

Current techniques can fall down at scale - I imagine things like various deduplication algorithms don't really work well when you have data split across a cluster and you can't do sorts etc. 

### Further Reading
- [[@chuDistributedDataDeduplication2016 - Distributed data deduplication]]
- [[@yakoutGuidedDataRepair2011 - Guided data repair]]
