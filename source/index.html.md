---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - JSON
  #- ruby
  #- python
  #- javascript

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true

code_clipboard: true
---

# Introduction
Sample EQL for Cost Calculator



# Cost Calculator
## Q1 - how much would phase 2 hiv cost

> API input

```json
{
    "data": {
        "eql": {
            "db_type": "activity",
            "date": {},
            "industry_ids": {
                "STUDY TITLE": []
            },
            "query_type": "find",
            "type": "transaction",
            "filter": {
                "and": {
                    "eq": {
                        "STUDY STAGE": ["Study"],
                        "PRODUCT TYPE": [],
                        "DISEASE AREA (KMR)": ["VIRAL"],
                        "METRIC TYPE": ["Total Cost Per Patient"],
                        "TRIAL PHASE GROUP": ["II"],
                        "LEVEL": ["DA"]
                    }
                }
            },
            "measure": {},
            "db_name": "jrd_activity_p1b_v1",
            "action": {
                "file": "calculator.R",
                "input_file_type": "json",
                "action_type": "cost_calculator",
                "end_point": "\/analytics\/v1\/cost_calculator\/",
                "variable_validation": false,
                "api": true,
                "type": "rcode",
                "is_refine_monte_carlo": false
            },
            "id": "leni_lumi-1b_ab56bce85c3b4f7c8ccc4d1ca8d11ab2_0",
            "visualization_type": "action",
            "dataset": "JNJ RND",
            "last_modified": "2020-08-10 19:03:23",
            "dimension": {},
            "jrd_ids": {
                "STUDY TITLE": ["200056 - TMC278 LA - PHIIB - POC COMBO STUDY - (DONE BY GSK - LATTE2)", "64281802DNG2001: PH IIA HUMAN CHALLENGE TRIAL (N=52)", "64281802DNG2002: PH IIA HUMAN CHALLENGE TRIAL DENV3 (N=52)", "64281802DNG2003 PH IIA TREATMENT SINGAPORE TRIAL (N=150)", "VAC52150EBL2001- PHASE II EU", "VAC52150EBL2002- PHASE II AFRICA", "VAC52150EBL2003- PHASE II WALTER REED STUDY (US\/AFRICA)", "VAC52150EBL2004 - PREVAC", "VAC52150EBL2005 - AFRICAN PEDIATRIC STUDY - IMI (N=100)", "VAC52150EBL2006 - REVOLVE UK", "VAC52150EBL2007 - AFRICAN HCW FEASIBILITY STUDY", "VAC52150EBL2008 - RESOLVE SENEGAL", "VAC52150EBL2009 - UGANDA STUDY"]
            },
            "group": []
        }
    },
    "api_key": "31d5aa982a5303c61653199ee325c16a",
    "api_secret": "0eee0253ba1a166e732d6c5e51f1ae25"
}
```

## Q1 - Intermediate Filter - how much would phase 2 hiv cost

The intermediate filter changed to Indication

> API input

```json
{
	"data": {
		"eql": {
			"db_type": "activity",
			"date": {},
			"industry_ids": {
				"STUDY TITLE": []
			},
			"query_type": "find",
			"type": "transaction",
			"filter": {
				"and": {
					"eq": {
						"STUDY STAGE": ["Study"],
						"INDICATION (KMR)": ["HIV\/AIDS"],
						"PRODUCT TYPE": [],
						"DISEASE AREA (KMR)": ["VIRAL"],
						"METRIC TYPE": ["FTE Cost Per Patient"],
						"TRIAL PHASE GROUP": ["II"],
						"LEVEL": ["IND"]
					}
				}
			},
			"measure": {},
			"db_name": "jrd_activity_p1b_v1",
			"action": {
				"file": "calculator.R",
				"input_file_type": "json",
				"action_type": "cost_calculator",
				"end_point": "\/analytics\/v1\/cost_calculator\/",
				"variable_validation": false,
				"api": true,
				"type": "rcode",
				"is_refine_monte_carlo": false
			},
			"id": "leni_lumi-1b_e0adc07879e4496599a531bc4b2015e3_0",
			"visualization_type": "action",
			"dataset": "JNJ RND",
			"last_modified": "2020-08-10 19:03:23",
			"dimension": {},
			"jrd_ids": {
				"STUDY TITLE": ["200056 - TMC278 LA - PHIIB - POC COMBO STUDY - (DONE BY GSK - LATTE2)"]
			},
			"group": []
		}
	},
	"api_key": "31d5aa982a5303c61653199ee325c16a",
	"api_secret": "0eee0253ba1a166e732d6c5e51f1ae25"
}
```


## Q2 - How much would p2 diabetes cost


> API input

```json
{
	"data": {
		"eql": {
			"db_type": "activity",
			"date": {},
			"industry_ids": {
				"STUDY TITLE": []
			},
			"query_type": "find",
			"type": "transaction",
			"filter": {
				"and": {
					"eq": {
						"STUDY STAGE": ["Study"],
						"PRODUCT TYPE": [],
						"DISEASE AREA (KMR)": ["DIABETES MELLITUS"],
						"METRIC TYPE": ["Total Cost Per Patient"],
						"TRIAL PHASE GROUP": ["II"],
						"LEVEL": ["DA"]
					}
				}
			},
			"measure": {},
			"db_name": "jrd_activity_p1b_v1",
			"action": {
				"file": "calculator.R",
				"input_file_type": "json",
				"action_type": "cost_calculator",
				"end_point": "\/analytics\/v1\/cost_calculator\/",
				"variable_validation": false,
				"api": true,
				"type": "rcode",
				"is_refine_monte_carlo": false
			},
			"id": "leni_lumi-1b_a500881906954c80ad13d860d9a9ec8c_0",
			"visualization_type": "action",
			"dataset": "JNJ RND",
			"last_modified": "2020-08-10 19:03:23",
			"dimension": {},
			"jrd_ids": {
				"STUDY TITLE": []
			},
			"group": []
		}
	},
	"api_key": "31d5aa982a5303c61653199ee325c16a",
	"api_secret": "0eee0253ba1a166e732d6c5e51f1ae25"
}
```

## Q2 - Intermediate Filter - How much would p2 diabetes cost

The intermediate filter changed to Indication

> API input

```json
{
	"data": {
		"eql": {
			"db_type": "activity",
			"date": {},
			"industry_ids": {
				"STUDY TITLE": []
			},
			"query_type": "find",
			"type": "transaction",
			"filter": {
				"and": {
					"eq": {
						"STUDY STAGE": ["Study"],
						"INDICATION (KMR)": ["DIABETES - TYPE I"],
						"PRODUCT TYPE": [],
						"DISEASE AREA (KMR)": ["DIABETES MELLITUS"],
						"METRIC TYPE": ["Total Cost Per Patient"],
						"TRIAL PHASE GROUP": ["II"],
						"LEVEL": ["IND"]
					}
				}
			},
			"measure": {},
			"db_name": "jrd_activity_p1b_v1",
			"action": {
				"file": "calculator.R",
				"input_file_type": "json",
				"action_type": "cost_calculator",
				"end_point": "\/analytics\/v1\/cost_calculator\/",
				"variable_validation": false,
				"api": true,
				"type": "rcode",
				"is_refine_monte_carlo": false
			},
			"id": "leni_lumi-1b_23020ec270934756a61e224601dbf900_0",
			"visualization_type": "action",
			"dataset": "JNJ RND",
			"last_modified": "2020-08-10 19:03:23",
			"dimension": {},
			"jrd_ids": {
				"STUDY TITLE": []
			},
			"group": []
		}
	},
	"api_key": "31d5aa982a5303c61653199ee325c16a",
	"api_secret": "0eee0253ba1a166e732d6c5e51f1ae25"
}
```


## Q3 - How much would p2 prostate cancer cost


> API input

```json
{
	"data": {
		"eql": {
			"db_type": "activity",
			"date": {},
			"industry_ids": {
				"STUDY TITLE": []
			},
			"query_type": "find",
			"type": "transaction",
			"filter": {
				"and": {
					"eq": {
						"STUDY STAGE": ["Study"],
						"PRODUCT TYPE": [],
						"DISEASE AREA (KMR)": ["MALE REPRODUCTIVE CANCER"],
						"METRIC TYPE": ["Total Cost Per Patient"],
						"TRIAL PHASE GROUP": ["II"],
						"LEVEL": ["DA"]
					}
				}
			},
			"measure": {},
			"db_name": "jrd_activity_p1b_v1",
			"action": {
				"file": "calculator.R",
				"input_file_type": "json",
				"action_type": "cost_calculator",
				"end_point": "\/analytics\/v1\/cost_calculator\/",
				"variable_validation": false,
				"api": true,
				"type": "rcode",
				"is_refine_monte_carlo": false
			},
			"id": "leni_lumi-1b_eedd4351536440499829406c3c2741f6_0",
			"visualization_type": "action",
			"dataset": "JNJ RND",
			"last_modified": "2020-08-10 19:03:23",
			"dimension": {},
			"jrd_ids": {
				"STUDY TITLE": ["212082PCR2007 PH2KOREA\/TAIWAN REG N=82PTS", "64091742PCR2001 AN OPEN LABEL PHASE 2 EFFICACY AND SAFETY STUDY OF NIRAPARIB IN CASTRATE MEN WITH PROGRESSIVE ADVANCED PROSTATE CANCER AND DNA-REPAIR ANOMALIES", "64091742PCR2002 A PH1B\/2 STUDY OF NIRAPARIB COMBINATION THERAPIES FOR THE TREATMENT OF MEN WITH PROSTATE CANCER", "ARN-509-001 PHASE IIA", "ARN-509-002 PHASE IIA"]
			},
			"group": []
		}
	},
	"api_key": "31d5aa982a5303c61653199ee325c16a",
	"api_secret": "0eee0253ba1a166e732d6c5e51f1ae25"
}
```