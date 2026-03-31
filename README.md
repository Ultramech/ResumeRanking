

# **Resume Ranking AI by Django** 🎯📄  

**AI-powered Resume Ranking System built with Django**  

## **📌 Overview**  
Resume Ranking AI is a Django-based web application that uses **Natural Language Processing (NLP) and Machine Learning (ML)** to analyze and rank resumes based on job descriptions. It helps recruiters efficiently filter and prioritize resumes based on skills, experience, and qualifications.  

## **🚀 Features**  
✅ **AI-Powered Resume Screening** – Automatically ranks resumes based on relevance to the job description.  
✅ **Multiple CV Upload** – Upload and analyze multiple resumes at once for batch processing.  
✅ **Skill Matching** – Extracts and compares candidate skills with job requirements.  
✅ **Experience & Qualification Analysis** – Evaluates work experience and education.  
✅ **Customizable Ranking Criteria** – Adjust weights for different parameters.  
✅ **PDF Parsing** – Supports PDF resume formats.  
✅ **Admin Dashboard** – Manage resumes, job descriptions, and ranking criteria.  
✅ **REST API Support** – Integrate with external HR systems.  

## **🔧 Installation & Setup**  
### **1️⃣ Clone the Repository**  
```bash
git clone https://github.com/Ultramech/ResumeRanking.git
cd ResumeRanking
```
### **2️⃣ Create & Activate Virtual Environment**  
```powershell
# Windows PowerShell
python -m venv myenv
.\myenv\Scripts\Activate.ps1

# Or use the provided script
.\activate_env.ps1
```

```bash
# Mac/Linux
python -m venv myenv
source myenv/bin/activate
```

### **3️⃣ Install Dependencies**  
```powershell
# In virtual environment (Windows PowerShell)
& "E:/Code Arena/Programming/Python/Django/RESUME_RANKING_AI/myenv/Scripts/python.exe" -m pip install -r requirements.txt
```

```bash
# In virtual environment (Mac/Linux)
pip install -r requirements.txt
```

### **4️⃣ Set Up Environment Variables**  
Create a `.env` file in the project root and add your Groq API key:
```
API_KEY=your_groq_api_key_here
```

### **5️⃣ Run Database Migrations**  
```powershell
# Windows PowerShell
& "E:/Code Arena/Programming/Python/Django/RESUME_RANKING_AI/myenv/Scripts/python.exe" manage.py migrate
```

```bash
# Mac/Linux
python manage.py migrate
```

### **6️⃣ Create a Superuser (Optional)**  
```powershell
# Windows PowerShell
& "E:/Code Arena/Programming/Python/Django/RESUME_RANKING_AI/myenv/Scripts/python.exe" manage.py createsuperuser
```

### **7️⃣ Start the Development Server**  
```powershell
# Windows PowerShell - Use the provided script
.\run_server.ps1

# Or run directly
& "E:/Code Arena/Programming/Python/Django/RESUME_RANKING_AI/myenv/Scripts/python.exe" manage.py runserver
```

```bash
# Mac/Linux
python manage.py runserver
```

Access the app at **http://127.0.0.1:8000/**  

## **💡 Multiple CV Upload Feature**  
The application now supports uploading multiple resumes at once:

1. **Select Multiple Files**: On the upload form, you can select multiple PDF files at once (Ctrl+Click or Cmd+Click)
2. **Batch Processing**: All selected resumes are analyzed simultaneously against the chosen job description
3. **Individual Results**: Each resume gets its own detailed analysis card showing:
   - Match Score
   - Skills Extracted
   - Years of Experience
   - Relevant Project Categories
4. **File Identification**: Each result displays the resume number and filename for easy identification

## **🎯 How to Use**  
1. Navigate to the home page
2. Select a job title from the dropdown
3. Click the file upload button and select one or multiple PDF resumes (Ctrl+Click to select multiple)
4. Click "Check Resume(s)" to analyze
5. View detailed analysis results for each uploaded resume
6. Results include match score, skills, experience, and project categories  

## **📂 Project Structure**  
```
Resume_Ranking_AI/
│── Resume_Ranking_AI/      # Main Django app
│── templates/              # Frontend templates
│── static/                 # CSS, JS, images
│── models.py               # Database models
│── views.py                # Business logic
│── serializers.py          # API serializers
│── resume_checker/         # AI resume processing logic
│── requirements.txt        # Dependencies
│── manage.py               # Django entry point
```


## **📌 Future Enhancements**  
✅ AI-based **Resume Summarization**  
✅ **Job Matching Recommendations**  
✅ **Dashboard with Data Analytics**  
