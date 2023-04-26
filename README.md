```
# Web Scraping Deployment on AWS

This repository contains the code to deploy a web scraping application on AWS using Flask and Beautiful Soup.

## Getting Started

These instructions will help you set up the project on your local machine for development and testing purposes.

### Prerequisites

- Python 3.6 or higher
- AWS Account
- AWS CLI tool
- Boto3 package
- Flask

### Installing

1. Clone the repository:
    ```
    git clone https://github.com/Ravi24242424/for_AWS_deploy_web_scrap.git
    ```

2. Change into the project directory:
    ```
    cd for_AWS_deploy_web_scrap
    ```

3. Install required packages:
    ```
    pip install -r requirements.txt
    ```

4. Set up AWS CLI tool with your access and secret keys. Please refer to [AWS CLI configuration](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html) for detailed instructions.

5. Update the `config.py` with your desired configurations (e.g., S3 bucket name).

6. Start the Flask server:
    ```
    FLASK_APP=app.py flask run
    ```

## Deployment

To deploy the application on AWS using Elastic Beanstalk, follow these instructions:

1. Install the Elastic Beanstalk CLI:
    ```
    pip install awsebcli --upgrade --user
    ```

2. Initialize the Elastic Beanstalk project:
    ```
    eb init -p python-3.6 myproject-elasticbeanstalk
    ```
3. Create a new environment for deployment:
    ```
    eb create myproject-env
    ```

4. After your environment is created and your application is deployed, open your browser and visit the URL in the format `http://myproject-env.eba-abcdefg123.us-region-1.elasticbeanstalk.com`, replacing the placeholder values accordingly.

5. To update the deployment with the latest changes after committing the changes, run:
   ```
   eb deploy
   ```

## Built With

- [Python](https://www.python.org/) - Programming Language
- [Flask](https://flask.palletsprojects.com/) - Web framework used
- [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - Web scraping library

## Author

- **Ravi Kumar** - [Ravi24242424](https://github.com/Ravi24242424)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
