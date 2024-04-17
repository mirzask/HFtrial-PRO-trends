# Methods

## ClinicalTrials.gov API

- Condition: **Heart Failure**
	- `AREA[Condition]"Heart Failure"`
	- Heart Failure MESH ID: `AREA[ConditionMeshId]D000006333`
	- Ancestor ID for Cardiovascular Disease
		- CVD: `AREA[ConditionAncestorId]D000002318`
		- Heart Diseases: `AREA[ConditionAncestorId]D000006331`
- Study Type: Interventional (Clinical Trial)
- Adults, All sexes
- Phase 3 or 4

## PROQOLID Database

- PROQOLID was accessed on 11/28/2023
	- `dplyr::distinct(proms, .keep_all=T)`

## Regular Expression Patterns

```python
p_nyha = r'\b(NYHA|New York Heart Association)\b'
p_bnp = r'((?<![h])BNP|(?i)natriuretic peptide)'
p_6mw = r'6MW|(?i)(6|six)\s*-?\s*(min(?:ute)?s?)\s*-?\s*(hall)?\s*-?\s*(wal)'
p_hf_event = r'(?i)(hospitalization|hospitalisation|urgent visit|urgent hf visit|hf event|heart failure event|worsening heart failure|worsening hf|unplanned admission|heart failure decompensation|re-admission|hospital admission|hosp)'
p_death = r'(?i)(death|mortality)'
p_ef = r'(LVEF|(?i)ejection fraction)'
```
