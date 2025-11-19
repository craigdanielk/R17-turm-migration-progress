Internal Migration Record

Turm Kaffee – Magento → Shopify Transformation

Technical Progress Log



1. System Overview



Fully automated pipeline for:

	•	Magento products

	•	Magento pages

	•	Magento collections

	•	Images & assets

	•	Product/category mapping



Pipeline phases: Phase 1 → Phase 8 + Hydra.



⸻



2. Full Phase Breakdown



Phase 1 – Product Export & Normalisation

	•	Full Magento export

	•	SKU, variants, metafields extracted

	•	Cleaning + normalisation

	•	Shopify-ready CSV generated

	•	Imported into Shopify



Phase 2 – Page Scraping

	•	Crawler fetched 199 pages

	•	HTML saved + indexed



Phase 3 – Cleaning & Liquid Preparation

	•	JS/CSS removed

	•	HTML purified

	•	Converted to Liquid-safe blocks



Phase 4 – Image Processing

	•	Downloaded internal images

	•	Rewrote paths → Shopify CDN

	•	Missing image audit created



Phase 5 – Page Import

	•	GraphQL importer built

	•	SEO field fix added

	•	191 pages created

	•	7 pages updated

	•	2 manually recreated



Phase 6 – Validation

	•	Page integrity checks

	•	Handle normalisation

	•	Image references audited



Phase 7 – Liquid Directive Rewriter

	•	Reprocessed all content

	•	All 199 pages import-ready

	•	Import completed



⸻



Phase 8 – The Hydra Phase (Collection System)



Initial Matching Attempts



Handle-based fuzzy matching → inconsistent.



Final Selected Approach: SKU Deterministic Matching

	•	Shopify products fetched via API

	•	Matched 1-to-1 by SKU to Magento products

	•	SKU assignments used to rebuild collection mapping

	•	100% match rate



Scripts created:

	•	phase8_sku_map_products.js

	•	phase8_sku_extract_collections.js

	•	phase8_sku_import_assignments.js



Outputs:

	•	phase8_sku_matched_products.json

	•	phase8_sku_final_assignments.json



Results:

	•	265 total products

	•	177 assigned to collections

	•	454 total collection assignments

	•	88 products intentionally unassigned (not in Magento categories)



⸻



3. Remaining Technical Steps



Technical

	•	Build final navigation structure

	•	Validate all custom page templates

	•	Image optimisation pass

	•	Map 88 unassigned products manually

	•	Complete template linking



Theme

	•	Generate missing German templates

	•	Import all content blocks

	•	Mega-navigation rebuild



QA

	•	Page QA

	•	Navigation QA

	•	Mobile responsiveness

	•	Performance audit

	•	Final fixes → Launch



⸻



4. Repository Notes

	•	/site_data/ – All extraction/processing data

	•	/shopify_theme/ – Pulled Shopify theme

	•	/logs/ – Validation & import logs

	•	/docs/ – Documentation folder



⸻



5. Status Summary

	•	Products: 100%

	•	Pages: 100%

	•	Collections: 100% created

	•	Assignments: 100% mapped deterministically

	•	Navigation: Pending

	•	Templates: Pending

	•	QA: Pending



System stable and deterministic.



⸻

