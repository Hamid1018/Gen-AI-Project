AI Resume & Job Match Assistant

An AI-powered resume analysis tool that compares a candidate's resume with a job description and generates a structured report containing matched skills, missing or unclear skills, resume improvement suggestions, interview topics, and evidence notes.

This project was built as a  Generative AI mini project using Python, Groq API, Prompt Engineering, and Structured Outputs.

🚀 Project Overview

Job seekers often spend a lot of time comparing their resumes with job descriptions and deciding what skills or experience to highlight.

The AI Resume & Job Match Assistant simplifies this process by allowing a user to provide:

A resume
A job description

The application sends both to an LLM and produces a structured analysis.

What the application provides
✅ Matched skills
⚠️ Missing or unclear skills
📝 Resume improvement suggestions
🎯 Interview preparation topics
🔎 Evidence notes explaining the analysis
🛡️ Rules designed to prevent invented experience
📦 Machine-readable JSON output

Important: This tool is designed to help candidates prepare applications. It does not make hiring decisions or predict whether a candidate will get a job.

🧠 Technologies Used
Technology	Purpose
Python	Application logic
Groq API	LLM inference
openai/gpt-oss-20b	Language model
Prompt Engineering	Controls model behavior
Structured Outputs	Produces predictable JSON
JSON Schema	Defines the response structure
🏗️ How It Works
                    ┌───────────────────┐
                    │   User Resume     │
                    └─────────┬─────────┘
                              │
                              │
                    ┌─────────▼─────────┐
                    │  Job Description  │
                    └─────────┬─────────┘
                              │
                              ▼
                   ┌─────────────────────┐
                   │   Groq LLM API     │
                   │                     │
                   │ Prompt + Rules +    │
                   │ Resume + Job Post   │
                   └──────────┬──────────┘
                              │
                              ▼
                  ┌──────────────────────┐
                  │ Structured JSON      │
                  │                      │
                  │ • Matched Skills    │
                  │ • Missing Skills    │
                  │ • Improvements      │
                  │ • Interview Topics   │
                  │ • Evidence Notes     │
                  └──────────┬───────────┘
                              │
                              ▼
                    Human-Readable Report
✨ Key Features
1. Resume and Job Comparison

The assistant compares the candidate's supplied resume with the requirements in a job description.

2. Evidence-Based Analysis

The model is instructed to use only information present in the supplied resume and job description.

It should not invent:

Skills
Employers
Certifications
Projects
Dates
Years of experience
Achievements
3. Missing Skill Detection

Requirements that are not clearly supported by the resume are reported as missing or unclear instead of being invented.

4. Resume Improvement Suggestions

The assistant provides practical suggestions for improving the current resume based on the job description.

5. Interview Preparation

The application identifies topics that the candidate may want to prepare for based on the job requirements.
