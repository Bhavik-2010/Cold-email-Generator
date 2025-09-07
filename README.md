# 📧 Cold Mail Generator
The Cold Email Generator is an intelligent automation tool built using Groq, LangChain, and Streamlit. It allows users to provide the URL of a company’s careers page, from which it automatically scrapes job postings and generates personalized cold emails tailored to the job description. The system also links relevant portfolio projects, retrieved from a vector database (ChromaDB), to strengthen outreach. 

**Imagine a scenario:**

Suppose Nike is hiring a Principal Software Engineer. Instead of spending heavy resources on hiring and training, a software development company like Atliq can directly pitch services. Using this tool, Atliq’s business development executive (say, Mohan) can generate a tailored cold email highlighting relevant expertise and portfolio links—within seconds.

**🔑 Key Highlights**

Automated Job Scraping: Extracts job postings directly from company career pages.

Personalized Emails: Crafts role-specific cold emails enriched with portfolio links.

High Performance: Leveraging Groq’s LPU inference engine, the system achieves 0.8 sec email latency, representing a 7× speedup compared to standard LLM APIs.

Accuracy in Targeting: Evaluated with 78% precision and 88% recall for RAG retrieval, ensuring high-quality matching of portfolio content with job descriptions.

End-to-End Deployment: Delivered as a full-stack Streamlit application, seamlessly integrating multiple APIs into an efficient workflow.

![img.png](imgs/img.png)

## Architecture Diagram
![img.png](imgs/architecture.png)

## Set-up
1. To get started we first need to get an API_KEY from here: https://console.groq.com/keys. Inside `app/.env` update the value of `GROQ_API_KEY` with the API_KEY you created. 


2. To get started, first install the dependencies using:
    ```commandline
     pip install -r requirements.txt
    ```
   
3. Run the streamlit app:
   ```commandline
   streamlit run app/main.py
   ```
   
