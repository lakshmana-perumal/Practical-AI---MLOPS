# Practical AI & MLOPS
**Brief Overview of MLOps**
What is MLOps?

MLOps is a framework for development , deployment  and Maintenance of Machine Learning Systems ( set of ML Models) . The term MLOps stands for Machine Learning Operations . MLOPS is combination of both ML systems and Operations .
MLOps is a core function of Machine Learning engineering, focused on streamlining the process of taking machine learning models to production, and then maintaining and monitoring them. MLOps is a collaborative function, often comprising data scientists, devops engineers, and IT.

![image](https://github.com/lakshmana-perumal/Practical-AI---MLOPS/assets/101124079/27c468ed-dfe9-4b89-ba84-90cfec819850)




What is the use of MLOps?
MLOps is a useful approach for the creation and quality of machine learning and AI solutions. By adopting an MLOps approach, data scientists and machine learning engineers can collaborate and increase the pace of model development and production, by implementing continuous integration and deployment (CI/CD) practices with proper monitoring, validation, and governance of ML models.

Why do we need MLOps?
Productionizing machine learning is difficult. The machine learning lifecycle consists of many complex components such as data ingest, data prep, model training, model tuning, model deployment, model monitoring, explainability, and much more. It also requires collaboration and hand-offs across teams, from Data Engineering to Data Science to ML Engineering. Naturally, it requires stringent operational rigor to keep all these processes synchronous and working in tandem. MLOps encompasses the experimentation, iteration, and continuous improvement of the machine learning lifecycle.

What are the benefits of MLOps?
The primary benefits of MLOps are efficiency, scalability, and risk reduction. Efficiency: MLOps allows data teams to achieve faster model development, deliver higher quality ML models, and faster deployment and production. Scalability: MLOps also enables vast scalability and management where thousands of models can be overseen, controlled, managed, and monitored for continuous integration, continuous delivery, and continuous deployment. Specifically, MLOps provides reproducibility of ML pipelines, enabling more tightly-coupled collaboration across data teams, reducing conflict with devops and IT, and accelerating release velocity. Risk reduction: Machine learning models often need regulatory scrutiny and drift-check, and MLOps enables greater transparency and faster response to such requests and ensures greater compliance with an organization's or industry's policies.


The span of MLOps in machine learning projects can be as focused or expansive as the project demands. In certain cases, MLOps can encompass everything from the data pipeline to model production, while other projects may require MLOps implementation of only the model deployment process. A majority of enterprises deploy MLOps principles across the following:
![image](https://github.com/lakshmana-perumal/Practical-AI---MLOPS/assets/101124079/cadbf6d4-45fc-40e7-8b75-205dfe4c37e9)

	• Exploratory data analysis (EDA)
	• Data Prep and Feature Engineering
	• Model training and tuning
	• Model review and governance
	• Model inference and serving
	• Model monitoring
	• Automated model retraining


What are the best practices for MLOps?

The best practices for MLOps can be delineated by the stage at which MLOps principles are being applied.

Exploratory data analysis (EDA) :
		 Iteratively explore, share, and prep data for the machine learning lifecycle by creating reproducible, editable, and shareable datasets, tables, and visualizations.
Data Prep and Feature Engineering: 
		Iteratively transform, aggregate, and de-duplicate data to create refined features. Most importantly, make the features visible and shareable across data teams, leveraging a feature store.
Model training and tuning:
		 Use popular open source libraries such as scikit-learn and hyperopt to train and improve model performance. As a simpler alternative, use automated machine learning tools such as AutoML to automatically perform trial runs and create reviewable and deployable code.
Model review and governance:
		Track model lineage, model versions, and manage model artifacts and transitions through their lifecycle. Discover, share, and collaborate across ML models with the help of an open source MLOps platform such as MLflow.
Model inference and serving:
		  Manage the frequency of model refresh, inference request times and similar production-specifics in testing and QA. Use CI/CD tools such as repos and orchestrators (borrowing devops principles) to automate the pre-production pipeline.
Model deployment and monitoring :
		Automate permissions and cluster creation to productionize registered models. Enable REST API model endpoints.
Automated model retraining:
 Create alerts and automation to take corrective action In case of model drift due to differences in training and inference data.

Credit : databricks.com

**DevOps versus MLOps**
DevOps is a popular practice in developing and operating large-scale software systems. This practice provides benefits such as shortening the development cycles, increasing deployment velocity, and dependable releases. To achieve these benefits, you introduce two concepts in the software system development:
• Continuous Integration (CI)
• Continuous Delivery (CD)
![image](https://github.com/lakshmana-perumal/Practical-AI---MLOPS/assets/101124079/13218c6e-8b1c-44fe-a306-ba0b380b264d)

An ML system is a software system, so similar practices apply to help guarantee that you can reliably build and operate ML systems at scale.
However, ML systems differ from other software systems in the following ways:
• Team skills:
	In an ML project, the team usually includes data scientists or ML researchers, who focus on exploratory data analysis, model development, and experimentation. These members might not be experienced software engineers who can build production-class services.
• Development:
	ML is experimental in nature. You should try different features, algorithms, modeling techniques, and parameter configurations to find what works best for the problem as quickly as possible. The challenge is tracking what worked and what didn't, and maintaining 	reproducibility while maximizing code reusability.
• Testing:
	Testing an ML system is more involved than testing other software systems. In addition to typical unit and integration tests, you need data validation, trained model quality evaluation, and model validation.
• Deployment:
	In ML systems, deployment isn't as simple as deploying an offline-trained ML model as a prediction service. ML systems can require you to deploy a multi-step pipeline to automatically retrain and deploy model. This pipeline adds complexity and requires you to 	automate steps that are manually done before deployment by data scientists to train and validate new models.
• Production:
	ML models can have reduced performance not only due to suboptimal coding, but also due to constantly evolving data profiles. In other words, models can decay in more ways than conventional software systems, and you need to consider this degradation. Therefore, 	you need to track summary statistics of your data and monitor the online performance of your model to send notifications or roll back when values deviate from your expectations.
 
ML and other software systems are similar in continuous integration of source control, unit testing, integration testing, and continuous delivery of the software module or the package. However, in ML, there are a few notable differences:
• CI is no longer only about testing and validating code and components, but also testing and validating data, data schemas, and models.
• CD is no longer about a single software package or a service, but a system (an ML training pipeline) that should automatically deploy another service (model prediction service).
• CT is a new property, unique to ML systems, that's concerned with automatically retraining and serving the models.

Credit: Google


