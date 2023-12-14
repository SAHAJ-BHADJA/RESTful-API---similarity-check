# RESTful API For Similarity Check Using Natural Language Processing

## INTRODUCTION

- Build a Similarity check API using NLP, run and deploy using Docker & Docker-compose. 

-----------------

### Documents similarity
Document similarity (or distance between documents) is a one of the central themes in Information Retrieval. How humans usually define how similar are documents? Usually documents treated as similar if they are semantically close and describe similar concepts. On other hand “similarity” can be used in context of duplicate detection. We will review several common approaches.

![imageSimilarity](https://miro.medium.com/max/1838/1*l-BZLW3JUHd1MZbNq1MjQA.png)

----------------------

#### OBJECTIVE

`The objective of this API is to handle Similarity of text (PLAGIARISM CHECK) `

## API ARCHITECTURE
| **API Endpoint**         | **URL(PATH)** | **Method** | **Parameters**                           | **Responses**                                                           |
|--------------------------|---------------|------------|------------------------------------------|-------------------------------------------------------------------------|
| Register a User          | `/register`   | POST       | `username` (string), `password` (string) | 200: OK, 301: INVALID USERNAME                                           |
| Detect Similarity of Docs | `/detect`     | POST       | `username` (string), `password` (string), `text1` (string), `text2` (string) | 200: OK (returns similarity), 301: INVALID USERNAME, 302: INVALID PASSWORD, 303: OUT OF TOKENS |
| Refill Tokens            | `/refill`     | POST       | `username` (string), `admin_pw` (string), `refill_amount` (integer)    | 200: OK, 301: INVALID USERNAME, 304: INVALID ADMIN_PW                    |

------------------
 

## Contributing 

 Please feel free to fork this package and contribute by submitting a pull request to enhance the functionalities.
 
 -------------------


### Thanks! SAHAJ BHADJA. 



