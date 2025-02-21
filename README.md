### **IT Asset Lookup - Telex Integration**  
📌 **Query IT asset details directly in Telex** using `/assetlookup <AssetID>`.  

---

## **🔹 Overview**  
This integration allows users to retrieve IT asset information from a Google Sheet by typing `/assetlookup <AssetID>` in a Telex channel.  

### **🔹 How It Works**
1. A user enters `/assetlookup LAPTOP123` in a Telex chat.  
2. Telex sends the request to the integration’s API.  
3. The API looks up `LAPTOP123` in the Google Sheet.  
4. The asset details are returned in the chat.  

---

## **📌 Installation Guide**
### **Step 1: Host the `integration.json` file**
1. Clone this repository:  
   ```sh
   git clone https://github.com/AbdurrahmanIdr/it-asset-lookup-integration.git
   ```
2. Deploy the `integration.json` file to a public URL (e.g., **Vercel, GitHub Pages, AWS S3**).  

### **Step 2: Add the Integration to Telex**
1. Go to **Telex > App Store > Custom Integrations**.  
2. Enter the hosted `integration.json` URL.  
3. Click **Install** and enable the integration.  

---

## **🛠 Configuration**
After installing, go to your **Telex Organization Settings** and set:  
- **Google Sheets API Key** (required)  
- **Google Sheet ID** (required)  

---

## **🚀 Usage Example**
```
User: /assetlookup LAPTOP123
Telex Bot: 🔍 Asset Found!
 - Status: In Use
 - Current User: John Doe
 - Location: IT Office
```

---

## **📂 Repository Structure**
```
📦 it-asset-lookup-integration
 ├── 📜 integration.json   # Telex integration configuration
 ├── 📜 README.md         # Project documentation
```

---
