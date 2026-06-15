# Postman API Automation Integration with Github Actions #

This repository is a demonstration for POC for integrating postman tests with github actions. The tests are written in Postman and they are executed on the VM with the help of Newman and newman-reporter-htmlextra

Github actions will trigger the project execution on every push to the main branch. You can also execute the project manually using workflow_dispatch. The project runs on a scheduled time with the help of the cron job.

HTML report is archieved and kept in the artifact section for the team to download it. Along with that they can view the report direct from the github page https://harivenkateshsj.github.io/Phoenix-Inwarranty-Flow/

The latest report is mailed to the team members using GMAIL SMTP

## Testing Coverage ##
1. Happy Flow Testing
2. Negative Testing and Edge Case Testing
3. Token Testing
4. Data Driven Testing with CSV
5. Schema Validation
6. Secrets Management with Github Secrets

## Tech Stack ##
1. Postman
2. Nodejs
3. Newman
4. Newman-Reporter-Htmlextra
5. Github Actions
6. Gmail SMTP
7. Github Pages
8. CSV for Data Driven Testing
9. AWS-EC2 instance for self hosted github runner

## Github Page ##
You can directly view the latest test report of the postman test at the Github Page Link: https://harivenkateshsj.github.io/Phoenix-Inwarranty-Flow/

# HTML Report #
The Report will be created in the newman folder
![Postman Report](https://github.com/harivenkateshsj/Phoenix-Inwarranty-Flow/blob/static-content/newman-report.png)
![Postman Report](https://raw.githubusercontent.com/harivenkateshsj/Phoenix-Inwarranty-Flow/static-content/newman-report.png)

## How to run the Project ? ##
You can run the Project on your local system for that:
1. Clone the project on Local System https://github.com/harivenkateshsj/Phoenix-Inwarranty-Flow.git
2. Install Node.js and NPM from
   https://nodejs.org/en
3. Install Newman using npm ```install -g newman```
4. Install Newman-reporter-htmlextra npm ```install -g newman-reporter-htmlextra```
5. Run the Newman Command:
   ```Newman run 'Inwarranty-flow Collection Copy.postman-collection.json'\ -e QA.postman-environment.json\-d testdata.csv\-r cli,htmlextra\--reporter-htmlextra-export ./newman/index.html```
## Project Structure ##
```
Phoenix Inwarranty Flow
├─ Inwarranty-flow collection Copy.postman_collection.json
├─ Inwarranty-flow collectionExternal.postman_collection
├─ QA.postman_environment.json
└─ testdata.csv

```

## About Me ##

Hello! I'm **Harivenkatesh**, an Automation Testing and DevOps professional with over **6 years of experience** in designing, developing, and maintaining **scalable**, robust test automation frameworks and CI/CD solutions.

### Technical Skills

* **UI Automation:** Selenium WebDriver, Playwright
* **API Testing:** Rest Assured, Postman
* **Mobile Automation:** Appium
* **DevOps & CI/CD:** Experience in automating build, test, and deployment workflows

I am passionate about delivering high-quality software through efficient test automation, continuous integration, and modern DevOps practices. I specialize in building **scalable, maintainable, and reliable** automation frameworks, optimizing testing processes, and enabling faster, more dependable software delivery pipelines.

You can connect me over:
![LinkedIN](https://www.linkedin.com/in/sjhari/)


