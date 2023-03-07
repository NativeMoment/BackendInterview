## BackendInterview

# Backend for Simple Face Detection Challenges

Select a task from Task#1 or Task#2. 

## Task#1 Simple Backend for Simple Face Detection

#### Requirements
We have face detection engine which consume webcam image from localhost.
However, we need to run engine in the high performance server. 

1. Such that, you must create a client which consume webcam and send data over HTTP to the engine that also consume data using HTTP server.

2. We should deploy (run) the API, Queue (not required), and Worker in different hosts.
   
3. You may use any backend framework.

4. You may use any queue (**not required**).

#### Extra points
We don't required these, but you may show your skills in these ways:
- clean and readable code
- good object oriented style
- apply HTTPS instead of HTTP
- any new technology
- message queue (**not required**)

## Task#2 Scalable Backend for Simple Face Detection

#### Requirements
1. Create an API as task#1 described, but it should received data in the json format and push data into a queue (**required**).

2. Create a worker that consume data from the queue (**required**).

3. We should start new workers (image consumer tasks) as many as need.

4. Store the result in a database.

#### Extra points
We don't required these, but you may show your skills in these ways:
- clean and readable code
- good object oriented style
- apply HTTPS instead of HTTP
- any new technology
- save the result in an object storage

## Task#3 Front-end for Simple Face Detection

#### Requirements
1. Create a web app or mobile app to visualize the results from task#1 or task#2

2. Should render detected faces in image, you may render in front-end or back-end

3. Should draw bounding boxes or circle in rendered images
   
4. Connect to bankend using API

#### Extra points
We don't required these, but you may show your skills in these ways:
- clean and readable code
- good object oriented style
- apply HTTPS instead of HTTP
- any new technology
- Use the native stacks or React, React Native stacks.

## ============
## Installation
run these command to install this project.

### 1. Clone repo
```bash
git clone https://github.com/ratthapon/face-detection
```

### 2. Setup virtual environment
```bash
python3 -m venv venv
```

### 3. Install dependencies
```bash
source venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Deployment


### 1. Load installed dependencies
```bash
source venv/bin/activate
```

### 2. Start engine in a terminal manner 
```bash
python3 face_detection_engine.py
```

-----------------------
# Backend for Simple Knowsledage backend

#### Task 1 [ GRAPH QL ]
1. Import data to database.

2. Change type primary key from "int" to "UUID" and make sturture for support 2 language.

3. Generate by ORM format output genaral method (GET POST PUT PATCH and DELETE) 
    ```
    GET — R(etrieve) 
    POST — C(reate) 
    PUT — U(pdate) 
    PATCH - U(pdate)
    DELETE — D(elete) 
    ```  

4. This able serch and filter.

5. Genarate Test Scipt for test API.

------------------------------------
        
#### Task 2 [ REST API ]
## Problem Description

ZSSN (Zombie Survival Social Network). The world as we know it has fallen into an apocalyptic scenario. A laboratory-made virus is transforming human beings and animals into zombies, hungry for fresh flesh.

You, as a zombie resistance member (and the last survivor who knows how to code), was designated to develop a system to share resources between non-infected humans.

## Requirements

You will develop a ***REST API*** (yes, we care about architecture design even in the midst of a zombie apocalypse!), which will store information about the survivors, as well as the resources they own.

In order to accomplish this, the API must fulfill the following use cases:

- **Add survivors to the database**

  A survivor must have a *name*, *age*, *gender* and *last location (latitude, longitude)*.

  A survivor also has an inventory of resources of their own property (which you need to declare when upon the registration of the survivor).

- **Update survivor location**

  A survivor must have the ability to update their last location, storing the new latitude/longitude pair in the base (no need to track locations, just replacing the previous one is enough).

- **Flag survivor as infected**

  In a chaotic situation like that, it's inevitable that a survivor may get contaminated by the virus.  When this happens, we need to flag the survivor as infected.

  An infected survivor cannot trade with others, can't access/manipulate their inventory, nor be listed in the reports (infected people are kinda dead anyway, see the item on reports below).

  **A survivor is marked as infected when at least three other survivors report their contamination.**

  When a survivor is infected, their inventory items become inaccessible (they cannot trade with others).

- **Survivors cannot Add/Remove items from inventory**

  Their belongings must be declared when they are first registered in the system. After that they can only change their inventory by means of trading with other survivors.

  The items allowed in the inventory are described above in the first feature.

- **Trade items**:

  Survivors can trade items among themselves.

  To do that, they must respect the price table below, where the value of an item is described in terms of points.

  Both sides of the trade should offer the same amount of points. For example, 1 Water and 1 Medication (1 x 4 + 1 x 2) is worth 6 ammunition (6 x 1) or 2 Food items (2 x 3).

  The trades themselves need not to be stored, but the items must be transferred from one survivor to the other.

| Item         | Points   |
|--------------|----------|
| 1 Water      | 4 points |
| 1 Food       | 3 points |
| 1 Medication | 2 points |
| 1 Ammunition | 1 point  |

- **Reports**

  The API must offer the following reports:

    1. Percentage of infected survivors.
    1. Percentage of non-infected survivors.
    3. Average amount of each kind of resource by survivor (e.g. 5 waters per survivor)
    4. Points lost because of infected survivor.
    5. Genarate Test Scipt for test API.

---------------------------------------

#### Task 3

Genarate Web Page for show data fron 2 task using HTTPS Protocal 

1. Run Task 1 and 2 and this task such as diiference host (recommend using Docker)

2. Create simple page for show and management 2 API over HTTPS Protocal

3. Able Create Read Update Delete data from API.
