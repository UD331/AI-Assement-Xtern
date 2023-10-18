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

The ethical implications of data collection, storage, and biases are far-reaching, with issues such as privacy, consent, and transparency being the main concerns. Altman and Saetra in their papers emphasize the importance of informed consent as a main principle in data collection. Data biases raise questions regarding discrimination, fairness and social justice, which Sparrow and Howard note are deeply problematic, potentially resulting in unjust practices. Ensuring transparency and accountability in data practices is another important matter, as it can help build trust and prevent misuse of data.  Finally, the ownership and control of data are major ethical considerations, as they are needed for protecting individuals from exploitation and abuse.

From a business perspective, the above data practices can have a significant impact on various fields. Companies that focus data ethics are more likely to enjoy a strong reputation and higher levels of trust, which Altman and Saetra suggest can be considered valuable currency in the economy. Conversely, failing to follow these ethical data practices can result in legal and regulatory risks, which as Sparrow and Howard point out, lead to fines and operational disruptions. Ethical data practices can also result in innovation by fostering a culture of customer-centricity, where customers are more willing to share their data when they trust its handling.

On the technical front, addressing ethical concerns related to data require us to ensure data quality and reduce biases. Secure data storage is critical to protect against breaches and unauthorized access. Furthermore, implementing data governance and compliance tools is necessary for meeting ethical and legal obligations. In summary, the ethical, business, and technical implications of data collection, storage, and biases help us realize the importance of responsible data practices that not only align with societal values but also lead to favorable business outcomes and require advanced technical solutions to address these challenges.The ethical implications of data collection, storage, and biases are profound. Altman and Saetra emphasize the importance of informed consent as a fundamental principle in data collection, while Sparrow and Howard highlight the risks of discrimination, fairness, and social justice in the presence of data biases. Ensuring transparency, accountability, and data ownership/control are also critical ethical considerations to prevent misuse and protect individuals from exploitation and abuse.

From a business perspective, adhering to ethical data practices enhances reputation and trust. Altman and Saetra suggest that trust is a valuable currency in the economy. Failing to do so can result in legal and regulatory risks, leading to fines and operational disruptions. Ethical data practices can also foster innovation and customer-centricity.

On the technical front, addressing ethical concerns requires ensuring data quality, reducing biases, and implementing secure data storage, as well as data governance and compliance tools to meet ethical and legal obligations.

## Model Outline

For our model outline, we decided to go with DecisionTreeClassifier as after a little bit of testing I found that Classification algorithms suited my question of predicting order based on major, university and school year, better than Regression Models. Then considering that our dataset is actually relatively small and we have multiple categorical variables, I decided to go with DecisionTree over RandomForest. After that it was a straightforward process of preprocessing the data by converting our variables into numerical format for the model to work on. Creating our test and training set from the database by using test/train split. We use the standard 80/20 split for the testing and training purpose. We then fit our DecisionTreeModel and save it using pickle before finally testing it on our custom input.

## Future Improvements

The model created is basic, and there is potential for significant progress. With more time and resources, deep learning techniques using libraries like TensorFlow or PyTorch could be explored. A broader and better dataset would be essential for training a more robust machine learning model. Various accuracy metrics and a team of testers could be engaged to assess model accuracy. Gathering public and private opinions would help determine the project's market viability and popularity.

