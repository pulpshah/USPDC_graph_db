# USPDC_graph_db

This repository contains graph database schemas for the Pulp Informational Object (PIO), Persuasive Resonance, credentials for Neo4j instance, and code to complete modeling.

##### `pkl`

All pickle files representing USPDC debates and their scores. Copied from PulpInternet/debate_analysis

##### `transcripts_json`

Raw JSON files of debate transcripts with only turn_number, speaker, role, content. Copied from PulpInternet/debate_analysis

##### `02-extract_number.ipynb`

Score generator that takes the `transcripts_json` files as input, annotates with scores, and produces `pkl` files. Kept here for reference. Copied from PulpInternet/debate_analysis

##### `dynamic_model.ipynb`

Given Neo4j credentials and pkl file, dynamically generate scores and create corresponding nodes as per the schema outlined in `Pulp Informational Object.json` .

As of 08/05/24, it only uses `pkl/June 27, 2024 Presidential Debate Transcript.pkl` for testing purposes.

##### `Neo4j Credentials.txt`

Credentials for Neo4j instances updated by `dynamic_model.ipynb` .

##### `Persuasive Resonance.json`

Schema for persuasive resonance. Import into arrows.app

##### `Pulp Informational Object.json`

Schema for Pulp Informational Object. Import into arrows.app



###### **08/05**

Technical loom outlining dynamic modeling: [Here](https://www.loom.com/share/f347b5de13b742c2a20e0537973c3d13?sid=cbf49fcd-ea40-45f1-ba67-fe93f6546e52)

Figma mentioned in loom: [Here](https://www.figma.com/board/9VAyY7WCof322uF9TRporp/Research-Scrap-JM-AM?node-id=0-1&t=5qFaQMGkyh2jY7GP-1)
