```

\documentclass[a4paper,11pt]{article}
\usepackage{graphicx}
\usepackage[left=0.7in, right=0.7in, top=0.7in, bottom=0.7in]{geometry}
\usepackage[usenames,dvipsnames]{xcolor}
\usepackage{enumitem}
\usepackage[hidelinks]{hyperref}
\usepackage{fontawesome}
\usepackage{titlesec}
\usepackage{array}
\usepackage{multicol}
\usepackage{fancyhdr}

% Color definitions
\definecolor{MainColor}{RGB}{30, 90, 150} % Professional blue
\definecolor{SubheaderColor}{RGB}{80, 80, 80} % Gray for subheaders

% Header styling
\titleformat{\section}
{\color{MainColor}\Large\bfseries}
{}{0em}{}[\color{MainColor}\titlerule]

% Spacing adjustments
\titlespacing{\section}{0pt}{14pt}{8pt}
\setlength{\parindent}{0pt}
\setlength{\parskip}{0.5em}

% Customize lists - increased spacing for better readability
\setlist[itemize]{leftmargin=6mm, topsep=2pt, itemsep=2pt, parsep=0pt}

% Customize hyperlinks
\hypersetup{
    colorlinks=true,
    linkcolor=MainColor, 
    urlcolor=MainColor,
    pdfborder={0 0 0}
}

% Define custom commands
\newcommand{\jobtitle}[2]{{\large\color{MainColor}\textbf{#1}} \hfill {\color{SubheaderColor}\textit{#2}}}
\newcommand{\daterange}[1]{{\color{SubheaderColor}\textit{#1}}}
\newcommand{\skill}[1]{{\small\textsf{#1}}}
\newcommand{\projecttitle}[1]{{\color{MainColor}\textbf{#1}}}
\newcommand{\techstack}[1]{{\color{SubheaderColor}\textit{Tech:} #1}}

\pagestyle{fancy}
\fancyhf{}
\renewcommand{\headrulewidth}{0pt}

\begin{document}

\pagestyle{empty} % No page numbers

% Header - cleaner with more space
\begin{center}
    \textbf{\color{MainColor}\LARGE Ramsai Jagadish Yenugadhati} \\
    \vspace{0.2cm}
    {\color{SubheaderColor}\large Data Science \& Cloud Technology Professional}
    \vspace{0.3cm}
    
    \href{https://ramsai170899.github.io/profile/}{\faGlobe\ Portfolio} \hspace{0.5cm}
    \href{https://www.linkedin.com/in/ram-sai-jagadish-yenugadhati-8909201b1}{\faLinkedinSquare\ LinkedIn} \hspace{0.5cm}
    \href{https://github.com/Ramsai170899}{\faGithub\ GitHub} \hspace{0.5cm}
    \href{mailto:ramsai.yj@gmail.com}{\faEnvelope\ ramsai.yj@gmail.com} \hspace{0.5cm}
    \href{tel:+918919790956}{\faPhone\ +91 8919790956}
\end{center}

\vspace{0.2cm}

% Professional Summary - more concise
\section*{\textcolor{MainColor}{Professional Summary}}
Results-driven Data Science professional with expertise in Machine Learning, Cloud Technologies, and Data Engineering. Proven track record of optimizing performance and implementing end-to-end solutions. Skilled in Python, R, PySpark, and AWS cloud services with a passion for solving complex data challenges and delivering actionable insights.

\vspace{0.2cm}

% Experience - better structured with more space
\section*{\textcolor{MainColor}{Professional Experience}}

\jobtitle{Actuarial Business Analyst}{CreditAccess Life Insurance}
\daterange{February 2024 - Present}
\begin{itemize}
    \item Engineered high-performance Python-based tools for critical business operations
    \item \textbf{Optimized Reserve Calculation Model}: Achieved \textbf{7x performance improvement} by reducing runtime from 3.5 hours to 30 minutes through advanced code optimization
    \item Collaborated with cross-functional teams to translate business requirements into technical solutions
\end{itemize}
\vspace{0.3cm}


\jobtitle{Actuarial Data Science Intern}{SSSIHL}
\daterange{November 2023 - January 2024 } 
\begin{itemize}
\item As a Data Science Intern, I integrated AWS services into a Kidney Disease Classification project. 
\item Used Amazon S3 for data storage, EC2 for scalable computing, and SageMaker for machine learning. The web application was deployed on EC2, CloudWatch was implemented for monitoring, and security was ensured through IAM
\item Demonstrated expertise in optimizing project efficiency and scalability through AWS integration.
\end{itemize}
\vspace{0.3cm}


\jobtitle{Software Engineer}{Bluezone International Inc}
\daterange{September 2022 - October 2023}
\begin{itemize}
    \item \textbf{AWS-Integrated Application Development}: Built sensor data acquisition system with AWS microservices
    \item Enhanced fingerprint pattern identification system with AWS Analytics for fraud detection
    \item Implemented real-time notification system with optimized sensor usage recommendations
    \item Performed critical bug fixes and feature enhancements for data collection tools
\end{itemize}

\vspace{0.3cm}

\jobtitle{Actuarial Data Science Intern}{Tech Actuarial}
\daterange{June 2022 - August 2022}
\begin{itemize}
    \item Developed insurance fraud detection model achieving \textbf{95\% accuracy} and \textbf{0.99 AUC}
    \item Applied SMOTE technique to address data class imbalance challenges
    \item Implemented Random Forest classifier optimized for fraud pattern identification
\end{itemize}

\vspace{0.2cm}

% Education - simplified
\section*{\textcolor{MainColor}{Education}}

\jobtitle{MSc Data Sciences and Computing}{CGPA: 7.2}
\daterange{Sri Sathya Sai Institute of Higher Learning, Andhra Pradesh | 2020 - 2022}

\jobtitle{Bachelor of Computer Applications}{CGPA: 7.0}
\daterange{Sri Sathya Sai Institute of Higher Learning, Andhra Pradesh | 2017 - 2020}

\vspace{0.2cm}

% Key Projects - selected most impressive ones
\section*{\textcolor{MainColor}{Key Projects}}

\projecttitle{Actuarial Data Science Project using PySpark} \\
\techstack{PySpark, GLMs, Neural Networks, Statistical Modeling}
\begin{itemize}
    \item Developed regression models for motor insurance claim estimation with \textbf{RMSE of 0.30 and MAE of 0.09}
    \item Implemented distributed computing for significant reduction in modeling time
\end{itemize}

\vspace{0.2cm}

\projecttitle{MNIST Digit Classification Web App} \\
\techstack{TensorFlow, Keras, Flask, CNN, HTML/CSS}
\begin{itemize}
    \item Built end-to-end web application for handwritten digit recognition achieving \textbf{98\% accuracy}
    \item Implemented data preprocessing pipeline handling 70,000 images with augmentation techniques
\end{itemize}

\vspace{0.2cm}

\projecttitle{End-to-End Diabetes Prediction System} \\
\techstack{Flask, Scikit-learn, LGBM Classifier, EDA}
\begin{itemize}
    \item Analyzed 100,000 patient records achieving \textbf{91\% accuracy} with ROC-AUC score of 0.91
    \item Implemented hyperparameter tuning to optimize model performance
\end{itemize}

\vspace{0.2cm}

\projecttitle{Multiclass Food Item Classification} \\
\techstack{CNN, TensorFlow, Transfer Learning, ResNet, Flask}
\begin{itemize}
    \item Built image classification system for 30 food categories using 11,000 training images
    \item Achieved \textbf{92\% accuracy} through transfer learning with ResNet architecture
\end{itemize}

\vspace{0.2cm}

% Publication - simplified
\section*{\textcolor{MainColor}{Publication}}
\textbf{International Journal of Emerging Technologies and Innovative Research} \\
"Estimation of Number of Claims in Motor Insurance using Generalized Linear Models and Artificial Neural Networks" \\
Paper ID: JETIR2206A01 - \href{https://www.jetir.org/view?paper=JETIR2206A01}{Link to Publication}

\vspace{0.2cm}

% Skills - better organized
\section*{\textcolor{MainColor}{Technical Skills}}

\begin{multicols}{2}
\textbf{Data Engineering \& Big Data}
\begin{itemize}[noitemsep]
    \item Hadoop, Spark, PySpark, Databricks
    \item AWS (EC2, S3, SageMaker, CloudWatch)
    \item Kafka, Cassandra, Docker
\end{itemize}

\textbf{Programming \& Analysis}
\begin{itemize}[noitemsep]
    \item Python, R, C++, Java
    \item Pandas, Statistical Analysis, ML/DL
    \item Power BI, Matplotlib, Seaborn
\end{itemize}

\columnbreak

\textbf{Web Development}
\begin{itemize}[noitemsep]
    \item Flask, React
    \item SQL, RDBMS
    \item Git, GitHub
\end{itemize}

\textbf{Certifications}
\begin{itemize}[noitemsep]
    \item Big Data Hadoop and Spark Developer
    \item Machine Learning
    \item Applied Data Science with Python
\end{itemize}
\end{multicols}

\end{document}



```
