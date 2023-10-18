# AI-Assessment-Xtern

This README contains the findings and explanations for the choices made during the assessment.

## Exploratory Analysis

For the exploratory analysis, the following results were obtained:

- Average Opening Time: 12.53 hours
- Unique Majors: 20
- Unique Universities: 10
- Unique Orders: 10

**Orders:**

- Sugar Cream Pie: 512
- Indiana Pork Chili: 510
- Cornbread Hush Puppies: 510
- Sweet Potato Fries: 508
- Ultimate Grilled Cheese Sandwich (with bacon and tomato): 503
- Indiana Buffalo Chicken Tacos (3 tacos): 496
- Indiana Corn on the Cob (brushed with garlic butter): 495
- Breaded Pork Tenderloin Sandwich: 494
- Fried Catfish Basket: 490
- Hoosier BBQ Pulled Pork Sandwich: 482

**Popular Orders by University:**

- Ball State University: Indiana Corn on the Cob...
- Butler University: Indiana Pork Chili...
- DePauw University: Indiana Buffalo Chicken Ta...
- Indiana State University: Hoosier BBQ Pulled ...
- Indiana University Bloomington: Ultimate Gril...
- Indiana University-Purdue University Indianap...
- Purdue University: Ultimate Grilled Cheese Sa...
- University of Evansville: Indiana Buffalo Chi...
- University of Notre Dame: Ultimate Grilled Ch...
- Valparaiso University: Sweet Potato Fries

**Popular Orders by Major:**

- Accounting: Indiana Corn on the Cob...
- Anthropology: Hoosier BBQ Pulled Pork Sandwich
- Astronomy: Ultimate Grilled Cheese Sandwich...
- Biology: Indiana Pork Chili
- Business Administration: Ultimate Grilled Cheese...
- Chemistry: Indiana Pork Chili
- Civil Engineering: Indiana Corn on the Cob...
- Economics: Indiana Pork Chili
- Finance: Indiana Buffalo Chicken Tacos...
- Fine Arts: Fried Catfish Basket
- International Business: Breaded Pork Tenderlo...
- Marketing: Breaded Pork Tenderloin Sandwich
- Mathematics: Ultimate Grilled Cheese Sandwich...
- Mechanical Engineering: Breaded Pork Tenderlo...
- Music: Fried Catfish Basket
- Philosophy: Fried Catfish Basket
- Physics: Ultimate Grilled Cheese Sandwich...
- Political Science: Sugar Cream Pie
- Psychology: Fried Catfish Basket
- Sociology: Fried Catfish Basket

The visualizations for these findings are available in the ipynb file.

Useful business use cases include identifying popular orders by university, enabling targeted menus and restaurants around university premises. Additionally, determining popular foods by major can help businesses create relevant targeted advertisements for students.

## Ethical Implications

The ethical implications of data collection, storage, and biases are profound. Altman and Saetra emphasize the importance of informed consent as a fundamental principle in data collection, while Sparrow and Howard highlight the risks of discrimination, fairness, and social justice in the presence of data biases. Ensuring transparency, accountability, and data ownership/control are also critical ethical considerations to prevent misuse and protect individuals from exploitation and abuse.

From a business perspective, adhering to ethical data practices enhances reputation and trust. Altman and Saetra suggest that trust is a valuable currency in the economy. Failing to do so can result in legal and regulatory risks, leading to fines and operational disruptions. Ethical data practices can also foster innovation and customer-centricity.

On the technical front, addressing ethical concerns requires ensuring data quality, reducing biases, and implementing secure data storage, as well as data governance and compliance tools to meet ethical and legal obligations.

## Model Outline

For the model outline, the DecisionTreeClassifier was chosen due to its suitability for predicting orders based on major, university, and school year. This classification algorithm proved better than regression models for the given question. Considering the relatively small dataset and multiple categorical variables, DecisionTree was preferred over RandomForest. The data was preprocessed by converting variables into numerical format, and the dataset was split into test and training sets using an 80/20 split. The DecisionTree model was fitted and saved using pickle before testing it on custom input.

## Future Improvements

The model created is basic, and there is potential for significant progress. With more time and resources, deep learning techniques using libraries like TensorFlow or PyTorch could be explored. A broader and better dataset would be essential for training a more robust machine learning model. Various accuracy metrics and a team of testers could be engaged to assess model accuracy. Gathering public and private opinions would help determine the project's market viability and popularity.

