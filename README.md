## SpaceOdyssey - Automated Radius Update Project

### Project Overview
The **SpaceOdyssey Automated Radius Update** project automates the updating of ad campaign radius on Google and Facebook Ads based on data in CSV files received via email. This solution was designed to help SpaceOdyssey dynamically target potential customers within specific geographic areas, adjusting ad radius according to weekday and weekend needs.

### Solution Summary
The project workflow consists of automated email monitoring, cloud-based data processing, API interactions with ad platforms, and data visualization:

1. **Automated Email Monitoring**:  
   - A Google Apps Script monitors the designated Gmail account for incoming emails containing the CSV file with ad radius data.
   - Upon detecting a new file, the script forwards the data to AWS for further processing.

2. **AWS Data Processing**:  
   - The CSV data is stored in an Amazon S3 bucket.
   - An AWS Lambda function processes the data and adjusts the radius for ads via the Google and Facebook Ads APIs.
   - AWS API Gateway exposes the Lambda function as a REST API, facilitating secure and efficient communication.

3. **Ad Campaign Updates**:  
   - Using Google Ads and Facebook Ads APIs, the system dynamically updates the radius settings of ad campaigns based on CSV instructions, optimizing ad reach based on weekday/weekend schedules.

4. **Data Visualization**:  
   - Amazon QuickSight is used to create a dashboard visualizing campaign performance, helping stakeholders understand the effectiveness of radius-based targeting.

### Project Documentation
1. **[Technical Specification](https://github.com/fmordy01/SpaceOdyssey-automated-radius/blob/3adde267aa57cc65503e7fb9f9903d6299b2cd1d/SpaceOdyssey%20-%20Technical%20specification.pdf)**: Detailed project requirements, setup, and technical solutions.
2. **[Client Response](https://github.com/fmordy01/SpaceOdyssey-automated-radius/blob/3adde267aa57cc65503e7fb9f9903d6299b2cd1d/SpaceOdyssey%20-%20Client%20response.pdf)**: Overview of the solution approach, phases, and timeline provided to the client.
3. **[Summary for Line Manager](https://github.com/fmordy01/SpaceOdyssey-automated-radius/blob/3adde267aa57cc65503e7fb9f9903d6299b2cd1d/SpaceyOdyssey%20-%20Summary%20for%20line%20manager.pdf)**: Concise project summary, including key risks, challenges, and mitigation strategies.

### Technologies Used
- **Cloud Services**: AWS Lambda, S3, API Gateway, IAM roles, Amazon QuickSight
- **Programming & Scripting**: Python, Google Apps Script
- **APIs**: Google Ads API, Facebook Ads API

### Key Learning and Challenges
This project strengthened my skills in cloud-based architecture, API integration, and data security principles. Working through challenges like API error handling, secure data storage, and integration complexities with third-party services was invaluable.


