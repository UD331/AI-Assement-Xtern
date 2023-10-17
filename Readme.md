# AI-Assement-Xtern
This Readme will contain the findings and explanations for the choices we made for the assessment.

1. For the exploratory analysis, we found the following results-
   Average Opening Time: 12.53 hours
   Unique Majors: 20
   Unique Universities: 10
   Unique Orders: 10

Orders-
   Sugar Cream Pie                                             512
   Indiana Pork Chili                                          510
   Cornbread Hush Puppies                                      510
   Sweet Potato Fries                                          508
   Ultimate Grilled Cheese Sandwich (with bacon and tomato)    503
   Indiana Buffalo Chicken Tacos (3 tacos)                     496
   Indiana Corn on the Cob (brushed with garlic butter)        495
   Breaded Pork Tenderloin Sandwich                            494
   Fried Catfish Basket                                        490
   Hoosier BBQ Pulled Pork Sandwich                            482

Popular Orders by University-
   (Ball State University, Indiana Corn on the Co...  
   (Butler University, Indiana Pork Chili)  
   (DePauw University, Indiana Buffalo Chicken Ta...  
   (Indiana State University, Hoosier BBQ Pulled ...  
   (Indiana University Bloomington, Ultimate Gril...  
   (Indiana University-Purdue University Indianap...  
   (Purdue University, Ultimate Grilled Cheese Sa...  
   (University of Evansville, Indiana Buffalo Chi...  
   (University of Notre Dame, Ultimate Grilled Ch...  
   (Valparaiso University, Sweet Potato Fries)

Popular Orders by Major-
  Accounting  (Accounting, Indiana Corn on the Cob (brushed ...
              Anthropology   (Anthropology, Hoosier BBQ Pulled Pork Sandwich)
                 Astronomy  (Astronomy, Ultimate Grilled Cheese Sandwich (...
                   Biology                      (Biology, Indiana Pork Chili)
   Business Administration  (Business Administration, Ultimate Grilled Che...
                 Chemistry                    (Chemistry, Indiana Pork Chili)
         Civil Engineering  (Civil Engineering, Indiana Corn on the Cob (b...
                          Economics                    (Economics, Indiana Pork Chili)
                   Finance  (Finance, Indiana Buffalo Chicken Tacos (3 tac...
                 Fine Arts                  (Fine Arts, Fried Catfish Basket)
   International Business  (International Business, Breaded Pork Tenderlo...
                Marketing      (Marketing, Breaded Pork Tenderloin Sandwich)
              Mathematics  (Mathematics, Ultimate Grilled Cheese Sandwich...
   Mechanical Engineering  (Mechanical Engineering, Breaded Pork Tenderlo...
                    Music                      (Music, Fried Catfish Basket)
               Philosophy                 (Philosophy, Fried Catfish Basket)
                  Physics  (Physics, Ultimate Grilled Cheese Sandwich (wi...
        Political Science               (Political Science, Sugar Cream Pie)
               Psychology                 (Psychology, Fried Catfish Basket)
                Sociology                  (Sociology, Fried Catfish Basket)

The visualizations for these findings are in the ipynb file.

Useful business use cases from this data include- finding out which orders are popular by University allowing business owners to make targeted menus and even targeted restaurants around the university premises. Morevoer, figuring out which food is popular by which major would result in businesses making relevant targeted advertisements for the students.

2. 3
3. For our model outline- I decided to go with DecisionTreeClassifier as after a little bit of testing I found that Classification algorithms suited my question of predicting order based on major, university and school year, better than Regression Models. Then considering that our dataset is actually relatively small and we have multiple categorical variables, I decided to go with DecisionTree over RandomForest. After that it was a straightforward process of preprocessing the data by converting our variables into numerical format for processing
