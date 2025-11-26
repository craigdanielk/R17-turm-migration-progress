R17 • Turm Kaffee Migration Progress Report
Magento → Shopify Migration

Status: In Progress
Updated: Current Sprint

Project Overview

This report outlines the full migration of Turm Kaffee’s Magento storefront into Shopify, covering completed tasks, current progress, and remaining deliverables required to activate the new Shopify Flow-theme site.

The migration objective is functional parity with UX/visual modernisation, not a 1:1 replica of the old Magento UI.

1. Completed Work
Product Migration

All core product data has been fully extracted, transformed, validated, and migrated.

Highlights

✔ Full Magento product catalogue exported
✔ Metadata, variant structures, SKU rules, content blocks — parsed & cleaned
✔ Shopify-ready CSV generated and validated
✔ All products successfully imported into Shopify
✔ Images mapped and assigned to correct variants

Page Migration

The complete Magento CMS content layer has been processed.

Highlights

✔ 199 Magento HTML pages scraped
✔ Content converted to Shopify-compatible HTML
✔ 191 pages automatically generated
✔ 7 pages repaired via retry logic
✔ 2 pages manually recreated (structural exceptions)

Image Processing

✔ All product & content images crawled
✔ Normalised for Shopify CDN
✔ High-resolution paths identified for import
✔ Image-set mapping prepared for Flow theme

2. Work in Progress
Store Structure Mapping

Rebuilding Shopify’s information architecture based on the Magento hierarchy.

Tasks Underway

• Extracting Magento category tree
• Mapping categories → Shopify automated collections
• Identifying reusable custom blocks or widgets
• Documenting dependencies between categories, products, URLs

Theme Integration (Flow Theme)

Analysing the Flow theme capabilities to align content, blocks, and metafields.

Tasks Underway

• Mapping Magento content → Flow sections
• Identifying new opportunities:
– content blocks
– product info modules
– dynamic metafield-driven components
• Defining page-level layout logic

Data Normalisation

Meta-layer cleanup before final import.

Tasks Underway

• Metafield namespace & key cleanup
• Deduplicating values
• Mapping category_ids to modern Shopify collection logic
• Preparing Matrixify import for metafields

3. Next Steps
Immediate Priorities
A. Pull & Analyse Remaining Magento Data

• Category tree
• URL rewrites
• CMS blocks & widgets
• Discounts / promotions
• Inventory
• Search terms
• Review data

(This will be automated through the batch.sh pull sequence.)

B. Complete Metafield Definitions & Import

• Finalise all product metafield definitions
• Validate types
• Bulk-import via Matrixify
• Confirm theme integration with Flow

C. Rebuild Shopify Navigation

• Derive top-level navigation from category tree
• Map CMS pages to Flow theme
• Build footer navigation, legal pages, contact pages

D. Recreate Collections System

• Automated collections (e.g., kaffe → arabica level, roast levels)
• Manual collections for curated sets
• Apply metafields for category_ids if useful

E. Implement Tracking & Marketing Tech

• GA4
• Google Ads conversions
• Meta Pixel
• Klaviyo onsite events

4. Launch-Phase Tasks
Polish & QA

• Full mobile & desktop review
• Theme block refinement
• Product content spacing & formatting
• Fix broken links
• Verify SEO structure
• Check URL rewrite mapping

Technical QA

• Inventory sync
• Checkout flow validation
• Payments configuration
• Shipping rules
• Tax configuration (CH + EU handling)

Content QA

• CMS layouts
• Product descriptions
• Metafield-driven sections
• Navigation logic
• Image quality control

5. Project Principles
Functional Parity First

Replicate what matters in Magento — improve everything else.

Modern Shopify Implementation

Use Flow theme features, not legacy Magento patterns.

Scalable Architecture

Structured metafields, collections, and content blocks must support future product expansion.

Automation Wherever Possible

Matrixify + n8n + internal tooling used to minimise manual labour.

6. Summary

The migration has passed the major technical milestones: product import, page processing, and asset transformation.
The next sprints focus on: Magento data extraction, Shopify structural rebuild, Flow theme integration, and metafield import.

Once the remaining data is normalised and the theme is populated, the final QA and tracking layer will position Turm Kaffee for a smooth, modern, scalable Shopify go-live.

