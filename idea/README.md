## Identification & Optical character recognition (OCR) for Structured Documents - SBI

Powered By - Microsoft Corporation Pvt Ltd.

### Problem being solved
Using OCR functionality of Microsoft Cognitive Services, we can extract text from images and documents.
Following things are supposed to be extracted:
- Obtain from document / image:
    - Document Identification
    - Customer / Account Identification
    - Structured Text within Document
    - Unstructured Text within Document
    - Photograph of Customer
    - Official Signature
    - Customer Signature
    - Document Attestation
### Approach taken to create the model
Explored Microsoft Cognitive Services API and it's competitor GCP Vision API.
Following things have been concluded on a sample data so far. 

Printed characters -> 1095 characters

Handwritten characters -> 141 characters

| Accuracy index |	Definition |
| ------------- | ------------- |
| Character recognition rate (%) |	Number of correctly recognized characters / Total number of characters in verification image * 100  |
| Number of noise |	Number of characters recognized as characters not included in the verification data  |

### Recognition accuracy of the entire document


| | Azure  | GCP |
| ----|------------- | ------------- |
|Character recognition rate|	99.75%|	98.62%  |
| Number of noise|	One character|	17 characters  |

	

### Recognition accuracy of handwritten characters

| | Azure  | GCP |
| ----|------------- | ------------- |
|Character recognition rate|	100.0%|	88.65% |
| Number of noise|	0 characters|	One character  |

### reason why your solution should be considered

- Proper documentation of the Azure Cognitive Services API for OCR related use case in banking for all needs mentioned below: 
    - document Identification
    - Customer Photograph
    - Customer Signature
    - Document Attestation
    - Structured Text
    - Unstructured Text
- Testing with real data will be done since I am already familiar with the process of OCR in banking
- Easy to use high level API will be written for easy integration with other applications and frameworks in banking. 
- API's will be ready to follow ISD protocol of banking. 

### Source code link for github
[SBI-OCR](https://github.com/avinash-mishra/sbi-ocr)

submitted by: [Avinash Mishra](https://github.com/avinash-mishra)

email: avinash.mishra@sbi.co.in

phone no. 7909409790