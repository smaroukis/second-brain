#course/active 
garden-topic::[[561 Electrical Engineering|Electrical Engineering]]
anki: [[Anki C215 Electronics]]
Tags: `#anki-todo`, `#todo/img`,  `#q`, `#todo/refactor`

Ref note: [[hayesLearningTheArtOfElectronics2016]] | [Online PDF](https://www.uvm.edu/~gpetrucc/courses/Chem219/Lectures/%5BTom_Hayes%3B_Paul_Horowitz%5D_Learning_the_Art_of_Ele(z-lib.org).pdf)

## TODOs

> [!NOTE]- TODOs
> ```query
> path:215-LAoE tag:#todo
> ```

## Folder Hierarchy
%% Begin Waypoint %%
- **[[01-DC-Circuits]]**
- **[[02-RC-Circuits✅]]**
	- [[02-Lab-RC-Circuits✅]]
	- [[RC Differentiator Circuit]]
	- [[RC Filters]]
	- [[RLC Filters]]
- **[[03-Diode-Circuits]]**
	- [[Example - Full Bridge Rectifier]]
- **[[04-Transistors-1✅]]**
	- [[Example - AC Coupled Emitter Follower Impedance Changer]]
	- [[Example - Development of Push Pull from Emitter Follower]]
- **[[05-Transistors-2]]**
	- [[Example - Differential Amplifier From Common-Emitter Transistor]]
- **[[06-Op-Amps-1-Ideal]]**
	- [[06-Examples-Op-Amps-1]]
	- [[06-Lab-Op-Amps-1]]
	- [[Example -  Diff-Amp Op-Amp 2]]
- **[[07-Op-Amps-2-Non-Ideal]]**
- **08-Op-Amps-3**
- **12-MOSFETs**
	- [[12L MOSFETs]]
	- [[12N MOSFETs]]
- [[215 LAoE Log and Dashboard]]
- [[Anki C215 Electronics]]

%% End Waypoint %%
## Queries/Views
- see more in [[215 LAoE Log and Dashboard]]

> [!TIP]+ Class/Lecture Notes
> ```dataview
> table status, Summary
> where contains(file.folder, this.file.folder) and contains(parent, [[215-LAoE]])
> sort file.name asc
> ```

## Summaries / Processed Garden Notes
```dataview
list from "200-Courses/215-LAoE"
where !contains(parent, [[215-LAoE]]) and !contains(file.name, "Lab") and !contains(file.name, "Example") and !contains(file.name, "215")
sort file.name asc
```
## Worked Examples
```dataview
list from "200-Courses/215-LAoE"
where contains(file.name, "Example")
sort file.name asc
```
## See Also
- Book: [[horowitzArtOfElectronics2015]]