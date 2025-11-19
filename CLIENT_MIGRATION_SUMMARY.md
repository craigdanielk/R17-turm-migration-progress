Turm Kaffee Migration Summary

Magento → Shopify Migration

Status: In Progress



1. Overview



This document summarises the full migration of Turm Kaffee's Magento store to Shopify.

It covers what has been completed, what is in progress, and what remains before launch.



2. Completed Work



Product Migration

	•	All products exported from Magento

	•	All metadata, descriptions, variants and SKU structures parsed and cleaned

	•	Shopify-ready CSV generated and imported

	•	All products now live inside Shopify



Page Migration

	•	199 Magento HTML pages scraped

	•	Cleaned and converted to Shopify-compatible HTML

	•	191 pages created automatically

	•	7 pages updated using retry logic

	•	2 pages manually recreated



Image Processing

	•	All products and content images crawled

	•	Internal images rewritten to Shopify CDN

	•	External/missing file audit generated



Collection Migration

	•	Magento categories analysed and normalised

	•	Shopify collections generated

	•	Final product–collection mapping rebuilt using SKU deterministic matching

	•	All collections created and products assigned



Phase 8: Product–Collection Mapping  

Status: Complete  

Notes:  

- 265 Shopify products mapped to Magento products by SKU (100% match rate)  

- 177 products with valid Magento category mappings assigned to their collections  

- 88 products correctly identified as having no collection in Magento  

- Single product skipped: `espresso-1000g` (no collection defined in Magento source data)  

- Mapping integrity verified through deterministic SKU-based resolution  

- Final mapping validated; system now structurally accurate  

---  

Phase 9:



Theme Analysis

	•	Theme fully analysed

	•	Missing page templates identified

	•	Template migration plan created



3. Work in Progress



Product Assignments



Some products require confirmation due to Magento data inconsistencies.

Automated retry running.

Manual confirmation list prepared.



Theme Template Setup

	•	German templates

	•	Utility pages (dailydeals, result, kurse, tee, baristatools, zubehoer, maschinen)



Navigation

	•	Rebuilding Shopify navigation to match Magento structure



4. Next Steps

	1.	Finalise product–collection assignments

	2.	Generate all missing theme templates

	3.	Import content blocks

	4.	Rebuild navigation

	5.	Full QA pass

	6.	Performance audit

	7.	Launch prep



5. Final Deliverables

	•	Fully migrated Shopify store

	•	All collections + products mapped

	•	All Magento pages recreated

	•	Navigation aligned

	•	Custom templates integrated

	•	Ready for client QA

