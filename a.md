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
\usepackage{tabularx}
\usepackage{tcolorbox}
\usepackage{fancyhdr}

% Color definitions
\definecolor{MainColor}{RGB}{30, 90, 150}
\definecolor{SubheaderColor}{RGB}{80, 80, 80}

% Header styling
\titleformat{\section}
{\color{MainColor}\Large\bfseries}
{}{0em}{}[\color{MainColor}\titlerule]

\titlespacing{\section}{0pt}{14pt}{8pt}
\setlength{\parindent}{0pt}
\setlength{\parskip}{0.5em}

% List styling
\setlist[itemize]{left=1em, label=--, itemsep=3pt, topsep=3pt}

% Hyperlink styling
\hypersetup{
    colorlinks=true,
    linkcolor=MainColor, 
    urlcolor=MainColor,
    pdfborder={0 0 0}
}

% Custom commands
\newcommand{\jobtitle}[2]{
  \begin{tabular*}{\textwidth}{@{\extracolsep{\fill}} l r}
    {\large\color{MainColor}\textbf{#1}} & {\color{SubheaderColor}\textit{#2}} \\
  \end{tabular*}
}
\newcommand{\skill}[1]{{\small\textsf{#1}}}
\newcommand{\projecttitle}[1]{{\color{MainColor}\textbf{#1}}}
\newcommand{\techstack}[1]{{\color{SubheaderColor}\textit{Tech:} #1}}

% Colored section box
\tcbset{enhanced, boxrule=0pt, colback=MainColor!10, sharp corners, left=6pt, right=6pt, top=4pt, bottom=4pt, boxsep=0pt}
\newcommand{\coloredsection}[1]{
  \vspace{0.6em}
  \begin{tcolorbox}
    \textbf{\large\color{MainColor} #1}
  \end{tcolorbox}
}

\pagestyle{fancy}
\fancyhf{}
\renewcommand{\headrulewidth}{0pt}

\begin{document}

\pagestyle{empty}

% Header
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

\coloredsection{Professional Summary}
Results-driven Data Science professional with expertise in Machine Learning, Cloud Technologies, and Data Engineering. Proven track record of optimizing performance and implementing end-to-end solutions. Skilled in Python, R, PySpark, and AWS cloud services with a passion for solving complex data challenges and delivering actionable insights.

\coloredsection{Professional Experience}

\jobtitle{Actuarial Business Analyst}{CreditAccess Life Insurance (Feb 2024 - Present)}
\begin{itemize}
    \item Engineered high-performance Python-based tools for critical business operations
    \item \textbf{Optimized Reserve Calculation Model}: Achieved \textbf{7x performance improvement} by reducing runtime from 3.5 hours to 30 minutes through advanced code optimization
    \item Collaborated with cross-functional teams to translate business requirements into technical solutions
\end{itemize}

\jobtitle{Actuarial Data Science Intern}{SSSIHL (Nov 2023 - Jan 2024)} 
\begin{itemize}
    \item Integrated AWS services into a Kidney Disease Classification project
    \item Used Amazon S3 for storage, EC2 for computing, SageMaker for ML; deployed on EC2 with CloudWatch monitoring and IAM security
    \item Improved scalability and project efficiency via cloud integration
\end{itemize}

\jobtitle{Software Engineer}{Bluezone International Inc (Sep 2022 - Oct 2023)}
\begin{itemize}
    \item Built sensor data acquisition system with AWS microservices
    \item Improved fraud detection with AWS Analytics-enhanced fingerprint recognition
    \item Delivered real-time sensor alerts with optimized system utilization
    \item Resolved critical bugs and delivered feature enhancements
\end{itemize}

\jobtitle{Actuarial Data Science Intern}{Tech Actuarial (Jun 2022 - Aug 2022)}
\begin{itemize}
    \item Developed insurance fraud detection model with \textbf{95\% accuracy} and \textbf{0.99 AUC}
    \item Applied SMOTE to resolve class imbalance
    \item Used Random Forest classifier for fraud pattern learning
\end{itemize}

\coloredsection{Education}

\jobtitle{MSc Data Sciences and Computing}{CGPA: 7.2}
\textit{Sri Sathya Sai Institute of Higher Learning, AP | 2020 - 2022}

\jobtitle{Bachelor of Computer Applications}{CGPA: 7.0}
\textit{Sri Sathya Sai Institute of Higher Learning, AP | 2017 - 2020}

\coloredsection{Key Projects}

\projecttitle{Actuarial Data Science Project using PySpark} \\
\techstack{PySpark, GLMs, Neural Networks, Statistical Modeling}
\begin{itemize}
    \item Developed regression models for motor insurance claim estimation with \textbf{RMSE of 0.30 and MAE of 0.09}
    \item Leveraged distributed computing to cut modeling time significantly
\end{itemize}

\projecttitle{MNIST Digit Classification Web App} \\
\techstack{TensorFlow, Keras, Flask, CNN, HTML/CSS}
\begin{itemize}
    \item Built web app for digit recognition with \textbf{98\% accuracy}
    \item Applied preprocessing and augmentation to 70,000 images
\end{itemize}

\projecttitle{End-to-End Diabetes Prediction System} \\
\techstack{Flask, Scikit-learn, LGBM Classifier, EDA}
\begin{itemize}
    \item Analyzed 100,000 records, achieving \textbf{91\% accuracy} and ROC-AUC of 0.91
    \item Tuned hyperparameters to enhance model performance
\end{itemize}

\projecttitle{Multiclass Food Item Classification} \\
\techstack{CNN, TensorFlow, Transfer Learning, ResNet, Flask}
\begin{itemize}
    \item Classified 30 food categories using 11,000+ images
    \item Reached \textbf{92\% accuracy} via ResNet-based transfer learning
\end{itemize}

\coloredsection{Publication}
\textbf{International Journal of Emerging Technologies and Innovative Research} \\
"Estimation of Number of Claims in Motor Insurance using Generalized Linear Models and Artificial Neural Networks" \\
Paper ID: JETIR2206A01 – \href{https://www.jetir.org/view?paper=JETIR2206A01}{Link to Publication}

\coloredsection{Technical Skills}

\begin{tabularx}{\textwidth}{X X}
\textbf{Data Engineering \& Big Data} &
\textbf{Web Development} \\
\begin{itemize}[noitemsep]
    \item Hadoop, Spark, PySpark, Databricks
    \item AWS (EC2, S3, SageMaker, CloudWatch)
    \item Kafka, Cassandra, Docker
\end{itemize}
&
\begin{itemize}[noitemsep]
    \item Flask, React
    \item SQL, RDBMS
    \item Git, GitHub
\end{itemize}
\\
\textbf{Programming \& Analysis} &
\textbf{Certifications} \\
\begin{itemize}[noitemsep]
    \item Python, R, C++, Java
    \item Pandas, Statistical Analysis, ML/DL
    \item Power BI, Matplotlib, Seaborn
\end{itemize}
&
\begin{itemize}[noitemsep]
    \item Big Data Hadoop and Spark Developer
    \item Machine Learning
    \item Applied Data Science with Python
\end{itemize}
\end{tabularx}

\end{document}






```
