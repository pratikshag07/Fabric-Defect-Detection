# Fabric-Defect-Detection
1. Introduction 
 Fabric production in the textile industry is made using knitting, weaving and nonwoven 
machines. Due to the fracture, bending, and abrasion on the needle in knitting and weaving 
machines, many fabric defects occur during production. Fabric defects are traditionally 
detected in quality control units at the end of the production process. This includes the steps 
of sending the fabric roll to the quality control unit, unwinding the roll, and monitoring the 
fabric by a quality control operator or an automation system. 
 
   When performing quality control and defect detection procedures by the control operator, 
natural situations such as tiredness, absent-mindedness, psychological problems, or 
drowsiness may reduce efficiency. This situation leads to uncertainties and incompatibilities 
in quality control. Automation systems are inevitable to minimize uncertainties in these 
systems as this affects customer satisfaction, trust and therefore finances in the textile industry, 
defect detection plays a crucial role in process diagnosis and improvement. However, fabric 
defect detection is still a process performed by the human eye, as methods that can work on 
the production line and provide fast and sufficient performance are not yet widespread enough. 
In this paper, a new texture feature extraction method that is faster, more accurate and 
unaffected by image rotation for fabric defect detection is proposed and its details are 
presented. 
 
   It is a new method and not a hybrid or a method improvement. It is not affected by the rotation 
of the fabric image. It is independent of the image orientation. The proposed feature extraction 
method has lower computational cost and works much faster than conventional texture feature 
extraction methods and provides higher accuracy performance. 

2. Project Objective 
In textile industry, fabric defect detection is considered as a challenging task as the quality and 
the price of any textile product are dependent on the efficiency and effectiveness of the 
automatic defect detection. Previously, manual human efforts are applied in textile industry to 
detect the defects in the fabric production process. Lack of concentration, human fatigue, and 
time consumption are the main drawbacks associated with the manual fabric defect detection 
process. 
In this method, a new texture feature extraction method is presented and its defect detection in 
textile industry is compared with traditional texture detection methods. In the study, texture 
feature extraction from image and pixel-based defect detection using these features were first 
performed. Instead of traditional or hybrid methods, a new feature extraction method is 
proposed in this study. The proposed IFV method is expected to be computationally low-cost 
and rotation invariant. To prove the rotation invariance, the patches used to pre-pare the dataset 
were rotated at random angles. Moreover, an attempt is made to demonstrate the use of low 
scale patches, which is the worst-case scenario for online work.  
Applications for defect detection in the textile industry are mainly model-based, transform
based, and statistical methods. Model-based methods are feature extraction with mathematical 
modelling and parameter estimation techniques from the image. The modelling process 
involves complex calculations. Despite high performance in these methods, it is slow in 
practice. Grey Level Co-occurrence Matrix (GLCM) is a second-order statistical method 
to extract textural properties of the image.  
In the last stage, contrast, dissimilarity, homogeneity, energy and correlation features 
are calculated The GLCM method is stated to be more successful in some cases of fabric 
defect detection than methods such as GFB or LBFE . In addition, applications with 
GLCM require a large amount of memory in the use of high-size frames, and feature 
extraction processing time increases. 
Local Binary Feature Extraction (LBFE) method has used in many applications such as 
face recognition and texture classification . It is one of the most commonly used 
method for defect detection in textile. The first step is the binarization process of 
surrounding pixels. Surrounding pixels are selected according to a user-specified 
radius. The binarization process is a comparison of the current pixel with surrounding 
pixels. In the second step result of binarization process values are multiplied with a 
coded matrix. The result of the process is the sum of multiplied matrix values. In some 
applications, it is used only because of binarization without using the multiplication 
part. The main advantages of applying LBFE are easy to implement and low 
computational cost. However, the performance of this method is very low in 
illumination changes and image rotation states. 
While GLCM, which is the most successful among the traditional methods in terms of accuracy, 
has an accuracy value of 0.808, the proposed IFV method has an accuracy value of 0.826. While 
LBFE, the fastest among the traditional methods extracts feature in 0.0827 ms on average, the 
proposed IFV method performs the same duty in 0.0461 ms on average. 
From this point of view, the proposed method works 55% faster than the fastest algorithm and 
provides 1.8% more accurate results. Accordingly, the proposed algorithm has an obvious 
superiority in defect classification compared to traditional methods and shows that it is more 
suitable for online defect detection processes. Apart from the prefabricated defect masks 
provided with the dataset, it shows that defective regions can also be detected from some 
experimental images. This shows that the system can perform better. The proposed method 
shows that it can be used in future studies for defect detection using these features were first 
performed. Instead of traditional or hybrid methods, a new feature extraction method is 
proposed in this study. The proposed IFV method is expected to be computationally low-cost 
and rotation invariant. To prove the rotation invariance, the patches used to prepare the dataset 
were rotated at random angles. Earlier traditional methods for fabric defect detection. 
The proposed method is supposed to be more efficient and faster than other methods. 
Accordingly, automatic fabric defect detection is necessary for the textile industry to reduce 
cost and increase productivity. To enhance the quality and to decrease the production cost of 
the final textile product, it is the current requirement that the inspection process must be done 
by using some industrial automation.

3. Feasibility Study: 
A feasibility study for a fabric defect detection project involves assessing various aspects to 
determine whether the project is viable and worth pursuing. Here's a breakdown of what such 
a feasibility study might entail: 
 
3.1 Technical Feasibility: 
• Assess the available traditional methods for fabric defect detection. This could 
include image processing algorithms and Deep Learning models. 
• Determine if the model is mature enough to reliably detect defects in fabrics. 
• Consider the hardware requirements for implementing the system. 
 
3.2 Operational Feasibility: 
• Data Management - Plan for data collection, storage, and preprocessing to ensure 
data quality and security. 
 Data Processing- Proper Implementation of traditional deep learning techniques. 
 Comparison with Existing Models: Analyze the compatibility of the proposed 
model with traditional models. 
 
3.3 Economic Feasibility: 
• Cost Analysis- Estimate the initial development costs, including hardware, 
software 
 
3.4 Legal Feasibility: 
• Determine if there are any regulatory requirements or standards that the fabric defect 
detection system must meet. 
• Assess potential legal issues related to intellectual property and liability. 
 Use of only authorized dataset for fabric defect detection. 
 Ensure that the proposed model complies with relevant industry standards, data 
privacy regulations, and safety requirements. 

4. Methodology/ Planning of work 
The preparation of the data set consists of two steps. Defects occupy very little space compared 
to the overall appearance of the entire fabric. Therefore, the dataset is cropped to reduce and 
balance the size. In the first step, the defect points were centered and a 100 × 100 pixel window 
was cropped around this point. In the second step, the binary error mask corresponding to the 
cropped window is coded according to the defect type. This process was performed for multi
label classification. The binary coded raw defect masks are shown in Fig. After the cropping 
process comes the feature extraction process used in the training and testing phase. In this part, a 
small part of the images were first used to create a balanced dataset. Traditional methods and the 
proposed method were used for feature extraction. The feature dataset for learning was generated 
by sampling known points on the image. Three defective and three defect free patches are 
randomly selected from the defective image cropped to 100 × 100 pixels and feature extraction 
was performed. In this study, 7 × 7 pixel sized patches were used. The proposed IFV method is 
expected to be rotation invariant. To prove the rotation invariance, the patches used to prepare the 
dataset were rotated at random angles. However, in some images of the dataset, the defects are as 
small as 1 pixel or no defect is present, which disturbs the balance of the output. When such 
situations occur in the image, these images are excluded from feature extraction. 

5. Tools/Technology Used: 
5.1 Minimum Hardware Requirements 
Hardware required for the development of the project. 
 CPU:  A modern multi-core processor (e.g., Intel Core i5 or equivalent) to handle the 
computational tasks efficiently 
 RAM:  Minimum 8GB RAM to ensure smooth processing 
 GPU: A dedicated GPU is not necessary for basic sentiment analysis but could be 
beneficial for more advanced machine learning tasks. 
 HDD: At least 128 GB SSD for faster data access and processing. 
5.2 Minimum Software Requirements 
Software required for the development of the project. 
 OS : Windows 10 
 Development Tools: PyCharm, Jupyter Notebook, Visual Studio Code 
 Database: SQL Server 
 Web Browser: Google Chrome 
 Libraries: Numpy, IO, OS, Flask, Keras, Pandas, Tensorflow
