## Step-by-Step Project Setup

### Step 1: Signing Up and Logging into IBM Cloud
1. Go to [https://cloud.ibm.com](https://cloud.ibm.com)
2. Sign in using your IBM SkillsBuild/Academic email.
3. Complete the email verification and login process.

---

### Step 2: Deleting Previous Resources (If Any)

1. From the IBM Cloud Dashboard, click on the **☰ Navigation Menu** in the top left corner.
2. Select **"Resource List"**.
3. From each category (Services, Runtime, Storage), review any old Watsonx or Object Storage resources.
4. Click on the 3-dot menu next to any unused resource and choose **Delete** to free up space and avoid quota issues.
5. Confirm deletion for each.

---

### Step 3: Creating Watsonx.ai Studio

1. From the IBM Cloud Dashboard, click the **search icon** 🔍.
2. Type **"Watsonx.ai studio"** and select it from the list.
3. Click **Create** and check the required box for terms & conditions.
4. Once the instance is created, click **Launch** to open Watsonx Studio.

---

### Step 4: Provision Watsonx.ai Runtime

1. Click **Provision Watsonx.ai Runtime** ➝ **Next** ➝ **Create**.
2. Runtime will be used later for AutoAI model building and deployment.

---

### Step 5: Create a New Project

1. Click **New Project** ➝ **Next**.
2. Name your project (e.g., `PMGSY Classification ML`).
3. Scroll down and click **Add** to choose a Free Plan.
4. Click **Continue**, then **Create**.
5. Under the **Manage tab**, associate your project with the Watsonx.ai runtime.

---

### Step 6: Upload Dataset

1. Click **Add to Project** ➝ **Data**.
2. Choose **Browse** and upload the `PMGSY_DATASET.csv` file.
3. Confirm that the dataset appears under your project’s assets.

---

### Step 7: Run AutoAI Experiment

1. In the project dashboard, click **“Build machine learning models automatically”**.
2. Provide an experiment name like `pmgsy_scheme_classifier`.
3. Select the uploaded dataset and click **Next**.
4. When asked if it's a time series, choose **No**.
5. For **prediction column**, select `PMGSY_SCHEME`.
6. Click **Run Experiment**.

---

### Step 8: Analyze AutoAI Leaderboard

1. The system builds multiple pipelines automatically.
2. Pipelines are ranked based on performance metrics (Accuracy, F1-Score, etc.).
3. Click **Swap View** to analyze models and metrics.
4. Select the best pipeline (usually Pipeline #1 or #2).

---

### Step 9: Save and Promote the Model

1. Click **Save As** ➝ **Model Asset** ➝ **Create**.
2. After saving, click **Promote to Space**.
3. Create a new **Deployment Space** and associate Watsonx.ai runtime.
4. Click **Promote** again to finalize promotion.

---

### Step 10: Deploy the Model

1. In the deployment space, click the model asset.
2. Click **New Deployment** ➝ Name it (e.g., `pmgsy_model_api`) ➝ **Create**.
3. Your model is now deployed as a REST API.

---

### Step 11: Test the Model

1. Click the **Test** button in the deployment dashboard.
2. Enter input values for project features such as:
   - `STATE_NAME`,
   - `DISTRICT_NAME,
   - `NO_OF_ROAD_WORK_SANCTIONED`,
   - `LENGTH_OF_ROAD_WORK_SANCTIONED`,
   - `COST_OF_WORKS_SANCTIONED`,
   - etc.
3. Click **Predict** to see the suggested PMGSY Scheme (e.g., PMGSY-II).

---

## Outcome

-The trained model accurately classifies projects into correct PMGSY categories.  
-Real-time API can now be integrated into monitoring dashboards.  
-Transparent, fast, and scalable classification system to support policy decisions.

---

## References

- [AI Kosh Dataset - PMGSY](https://aikosh.indiaai.gov.in/web/datasets/details/pradhan_mantri_gram_sadak_yojna_pmgsy.html)
- [IBM Cloud](https://cloud.ibm.com/)
- [IBM Watson Studio Docs](https://dataplatform.cloud.ibm.com/docs)

---

## Acknowledgements

Special thanks to **AICTE**, **Edunet Foundation**, and **IBM SkillsBuild** for the mentorship and cloud infrastructure support.

---
