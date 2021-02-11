# Input/Output Description

> Note: Data at the provider level (each bullet point is a field); all keys must be present, values may be null when specified
- Providers.csv (_REQUIRED_):

|        Column       | Column Required?  |               Meaning                    |
|---------------------|-------------------|------------------------------------------|
| prov_id             |         Y         | Provider ID (NPI)                        |
| prov_spec           |         N         | Provider Specialty                       |
| proc_code           |         Y         | Procedure code (HCPCS, CPT, ICD10, etc.) |
| proc_code_type      |         Y         | Code type                                |
| diag_code           |         Y         | Diagnostic code                          |
| diag_code_type      |         Y         | Diagnostic code type (ICD10 or ICD9)     |--------------------------------------------------------------------------------------
	
- Output: a JSON list of objects contaning, for each record in the original orderthe following fields:
	- prov_ID        : Provider ID                      
	- prov_clust      : Procedure code                                                                 
	 
 - Reference file: sample.zip.out	
	
