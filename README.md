# CV_Evaluation_Using_LLM
This repo contains code related to Evaluation of a CV / Resume based on the Job Description

This code file uses LangChain , Google GenAI ,  PyMuPDF libraries to build a system that can Evaluate a Resume based on the Job Description given to him. This system ranks the system from 1-10 where 1 being the lowest and 10 being the highest.

This system also specify a small reason for the given score.

The file contains the code :
llm = ChatGoogleGenerativeAI(model="gemini-2.0-flash",
                             verbose=True,
                             temperature=0.0,
                             google_api_key=userdata.get("GOOGLE_API_KEY"))

which describes that Google Gemini 2.0 Model is used. Temprature is set to 0 to specify that LLM should strictly focus on the given Job Description and does not creativeness.

This code defines a function extract_text_from_pdf(pdf_path) that gets the path of file as a parameter and then reads all the data of pdf and store it in a variable.


