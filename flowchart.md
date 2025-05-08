```mermaid
graph TD;
   A[Receive returns from courier companies] --> B[Returns from Canada or US];
   B --> C[Companies in Canada: Wholesale, Tsaac Technologies, Science Resource];
   B --> D[Companies in US: Wholesale, Vision Scientific, Parco, Jackson Scientific];
   C --> E[Fill out return items for import form];
   D --> E;
   E --> F[Check all returns and record status];
   F --> G[Quality control];
   G --> H[QC Pass → New Packing];
   G --> I[QC Fail];
   I --> J[Discard];
   I --> K[Lack of parts/boxes → Reorder to China];
   K --> L[Place in repair area];
   L --> F;
   H --> M[Back to stock];
   M --> N[Input computer records];
   N --> O[Update inventory];
