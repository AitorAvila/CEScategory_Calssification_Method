# Fair Use Policy
Users can freely download the documents in this site on terms and conditions as required below. It is not necessary to inform us. We would like to support your scientific and/or educational activity. Please do not hesitate to contact us anytime. 
##### [Requests]
-Users are requested to clarify the method provider and/or reference in their papers.

-If the purpose of use is not your scientific or educational activity, please consult with us in advance.
By downloading this template, one is assumed to agree to the terms of our Fair Use Policy.
# Template content description
The Excel template attached to this repository can be used to classify photos into both main and secondary Cultural Ecosystem Services (CES) categories, based on their content. To use this template, it is important that the content of each photograph has been previously tagged, preferably with trained software such as [Google Cloud Vision API](https://cloud.google.com/vision), and that all individual tags have been categorized into a specific CES category (instructions in the associated paper). Detailed explanations to this method were published in our paper from [MethodsX journal](https://www.journals.elsevier.com/methodsx).
## 1. Template sheets:
* __Main_category_assignation__: This is the spreadsheet where occurs the assignment of main CES categories to the previously tagged photographs.
* __Secondary_category_assignation__: This is the spreadsheet where occurs the assignment of secondary CES categories to the previously tagged photographs.
* __Join_table__: This is the spreadsheet that contains a join table used for the calculations of the other two spreadsheets.
## 2. Template fields:
* __ID_img__: unique identifier of each image.
* __Catx__: different CES categories used for the classification.
* __Numerical values of each column of Catx__: sum of the scores (sum_score) of each CES category present in each photograph (instructions in the associated paper).
* __MaxValue__: maximum value of “sum_score” of CES categories. 
* __PositionMaxValue__: position that “MaxValue” occupies in the table.
* __Main_CES_category__: main CES category that is finally assigned to each photograph.
* __SecondMaxValue__: second highest value after “MaxValue”.
* __PositionSecondMaxValue__: position that “SecondMaxValue” occupies in the table.
* __"MaxValue"-"SecondMaxValue"__: numerical difference between “MaxValue” and “SecondMaxValue”.
* __50%of_MaxValue__: half of “MaxValue”.
* __("MaxValue"-"SecondMaxValue")-"50%of_MaxValue"__: numerical difference between "MaxValue"-"SecondMaxValue" and 50%of_MaxValue.
* __ColumnR_is_negative?__: this field checks if the result of ("MaxValue"-"SecondMaxValue")-"50%of_MaxValue" is negative or not. if it is negative, a secondary CES category will be assigned.
* __Secondary_CES_category__: secondary CES category that is finally assigned to each photograph. If “FALSE” appears, it means that the photograph does not require a category.
# Contact information
Aitor Àvila, aitor.avila@urv.cat , Universitat Rovira i Virgili, Spain. 
