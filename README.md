# Azure Batch Support Training – Lab 2

## Assessment Instructions

### Overview
In this lab, you will deploy an ARM template that provisions multiple resources in your Azure subscription. It is **highly recommended** that you create a new resource group for this deployment to ensure easier cleanup after the assessment.

### Assessment Steps

1. **Deploy the ARM template.**  
   - You may be prompted to specify a resource group for the deployment.  
   - **Creating a new resource group is recommended** to facilitate cleanup.  

2. **Navigate to the Batch account.**  
   - Locate the **Batch account** named **`azurebatchtrnlab2`** in the Azure portal.  

3. **Access the Pools tab.**  
   - In the Batch account, go to the **Pools** tab.  

4. **Inspect the pool details.**  
   - Select the **`trnlab2pool`**, which should have **1 dedicated node** (SKU: `STANDARD_D2S_V3`).  

5. **Review the Overview and Nodes tabs.**  
   - On the **Overview** page, you should see an **error message**.  

### Assessment Tasks

1. **Analyze the Overview Page**  
   - Identify and diagnose the error message displayed.  
   - Provide a technical explanation of the issue.  

2. **Investigate the Nodes Tab**  
   - Examine the information presented.  
   - Do you notice anything unusual?  
   - **Hint:** Return to the **Batch account page**, navigate to the **Pools** tab, and then revisit the **Overview** and **Nodes** pages within the pool.  

3. **Root Cause Analysis & Resolution**  
   - Explain the underlying reason for the error.  
   - Describe the steps required to resolve the issue.  

### Conclusion
Once you have diagnosed the issue and identified the resolution steps, be prepared to discuss your findings and justify your proposed solution.

---

## Deployment Instructions

To deploy the ARM template, follow these steps:

1. **Clone this repository** (if working locally):
   ```sh
   git clone https://github.com/Walter-B-Jr/updated_azbatchlab2.git
   cd updated_azbatchlab2

   az deployment group create --resource-group <YourResourceGroup> --template-file azure_batch_template.json

