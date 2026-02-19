Project Overview: FlipVision AI
FlipVision AI is a high-velocity, spatial computing solution designed for the liquidation and resale industry. By merging wearable hardware with localized artificial intelligence, the project transforms the chaotic process of "bin diving" and pallet processing into a streamlined, automated workflow.
________________________________________
The Core Components
•	Hardware: HeyCyan Smart Glasses serve as the "Eyes," providing a hands-free interface for capturing product data, manifests, and condition media.
•	The Persona: Bin Store Betty is the AI voice and visual avatar. She lives on the edge (the phone) and provides real-time expert guidance, pricing alerts, and "BOLO" (Be On the Look Out) notifications via audio and XR overlays.
•	The Brain: Google AI Edge & ML Kit drive the on-device intelligence. This allows for instant barcode scanning, OCR (text recognition) of manifests, and product categorization without needing a stable Wi-Fi connection.
•	The Muscle: n8n Automation handles the heavy lifting of business logic. It bridges the gap between a scanned item and a live eBay listing, accounting entry, or inventory update.
________________________________________
Tiered Service Model
The project is structured to capture both the hobbyist and the enterprise liquidation market:
Feature	FlipVision Base	FlipVision Pro
Sourcing	Hands-free barcode/product lookup	Advanced manifest & document OCR
Intelligence	Local RAG (Offline sales history)	Global Sync (Full business analytics)
AI Interaction	General AI Chat with Betty	Strategic "Buy/Pass" Profit Analysis
Automation	Local media & history logs	Full n8n integration (Auto-eBay drafts)
________________________________________
Technical Architecture
The app is built on Android 14+ using the Jetpack XR Framework. This allows the interface to transcend a flat screen, placing data panels and pricing tags directly into the user's field of vision using spatial anchoring.
1.	Data Ingestion: The HeyCyan SDK pipes video frames to a VisionAnalyzer.
2.	Local Inference: ML Kit extracts the UPC or text; Google AI Edge converts it into a vector for a Local RAG search against an SQLite database.
3.	Betty's Feedback: The app triggers a Text-to-Speech (TTS) response or an XR "Glimmer" overlay with the result.
4.	Sync Queue: For Pro users, the data is queued and pushed to an n8n webhook once connectivity is established.

