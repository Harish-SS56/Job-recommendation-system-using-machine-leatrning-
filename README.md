Job Recommendation System:

This project is a Streamlit-based Job Recommendation System designed to assist both job seekers and recruiters in simplifying the hiring process. Leveraging NLP techniques, TF-IDF similarity, and real-time job APIs, this application provides tailored recommendations and insights.

 Features

Job Seeker Module
- Upload CVs: Users can upload multiple CVs in PDF format, which are parsed to extract relevant text and skills using NLP.
- Skill Extraction: Identifies key skills and keywords from the uploaded CVs using **SpaCy** NLP.
- Job Recommendations:
  - From a local dataset of job listings using TF-IDF Vectorization and Cosine Similarity.
  - Real-time job openings fetched via the Jooble API based on extracted skills.
- Interactive CV Display: CVs are displayed in an embedded PDF viewer, with an option to download them.

Recruiter Module
- Job Description Analysis: Recruiters can input a job description, which is processed to extract key features.
- CV Matching: Matches uploaded CVs to the job description using **TF-IDF Vectorization** and ranks them based on similarity scores.
- Top Recommendations: Displays top-matching CVs with their similarity scores and allows recruiters to view, download, or save the results.
- Downloadable Reports: Export similarity scores and rankings as a text file.

Core Technologies
- Streamlit: For building an interactive and user-friendly web application.
- NLP Tools:
  - SpaCy: Skill extraction from CVs and job descriptions.
  - NLTK: Text preprocessing, tokenization, stopword removal, and lemmatization.
- TF-IDF Vectorization: To compute similarity between job descriptions and CVs.
- Cosine Similarity: For ranking CV-job matches.
- Jooble API Integration: For real-time job recommendations.
- PyMuPDF (Fitz): For extracting text from PDF files.
- Pandas: For managing and analyzing job and CV data.

 Installation
1. Clone the repository:
   
   git clone https://github.com/your_username/job-recommendation-system.git
   
2. Navigate to the project directory:

   cd job-recommendation-system
   
3. Install dependencies:
   
   pip install -r requirements.txt
   
4. Run the Streamlit app:
   
   streamlit run app.py
   

 Usage
1. Select your role:
   - Job Seeker: Upload your CV and get tailored job recommendations.
   - Recruiter: Input a job description and get the best-matching CVs from the uploaded collection.
2. View, download, or export results for further use.

 Future Enhancements
- Integration with additional APIs (e.g., LinkedIn Jobs, Google Jobs).
- Advanced NLP models for better skill extraction and matching.
- Support for additional file formats (e.g., Word documents).
- Machine Learning-based ranking for improved recommendations.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
