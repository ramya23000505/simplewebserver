# EX01 Developing a Simple Webserver
## Date:

## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation.

### Step 2:
Design of webserver workflow.
### Step 3:
Implementation using Python code.

### Step 4:
Serving the HTML pages.

### Step 5:
Testing the webserver.

## PROGRAM:
Developed by: RAMYA R

Register No: 212223230169
```
content='''
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <style>
        .row1 {
             height: 50px;
             background-color: #f3f3f3;
             display: flex;
             place-items: center;
        }
        i {
            color: #cc324b;
            font-size: 15px;
        }
        a{
            color: #cc324b;
            text-decoration: none;
            font-size: 15px;
            font-family: ;
            padding: 10px;
        }
        a:hover {
            color:grey;
        }
        i:hover{
            color: grey;
        }
.trapezoid{
    background-color: gainsboro;
}
    </style>
</head>
<body>
    <div class="row1 p-3" >
        <div style="width: 40%">                                        
            <a href=""><i class="bi bi-twitter" ></i></a>
            <a href=""><i class="bi bi-youtube"></i></a>
            <a href=""><i class="bi bi-facebook" ></i></a>
            <a href=""><i class="bi bi-linkedin"  ></i></a>
            <a href=""><i class="bi bi-pinterest" ></i></a>
            <a href=""><i class="bi bi-whatsapp"></i></a>
            <a href=""><i class="bi bi-instagram"></i></a>
            </div>

        <div style="width: 40%;">
        <a href="">NDTV</a> <i class="bi bi-three-dots-vertical"></i>
        <a href="">WORLD EDITION</a> <i class="bi bi-three-dots-vertical"></i>
        <a href="">IPL 2024</a> <i class="bi bi-three-dots-vertical"></i>
        <a href="">MOVIES</a> <i class="bi bi-three-dots-vertical"></i>
        <a href="">GAMES</a> 
        </div>
        <div style="width: 20%">
        <div style="border: 3px solid; border-radius: 20px">
          <i class="bi bi-search"></i>
          <input   type="search text" style="height:30px; background-color:#f3f3f3; border: 0px; outline: none;" ; placeholder="Search" / >
        </div>
    </div>
    </div>
    <div class="row p-3 ">
        <div class="col-3" style="background-color: gainsboro;">
            <img src="new sports ex1.svg" style="width: 300px", height="100px">
        </div>
        <div class="col-9"; style="display: flex; background-color: gainsboro;">
       
        <a href="">Cricket</a>
        <a href="">About</a>
        <a href="">Football</a>
        <a href="">Tensis</a>
        <a href="">Hockey</a>
        <a href="">Kabaddi</a>
        <a href="">Batmiton</a>
        <a href="">Racing</a>
        <a href="">Westling</a>
        <a href="">Boxing</a>
        <a href="">Shouting</a>
        </div>
       
    </div>
    <div class="row">
        <div class="col-6">
            <div style="display: flex">
                <div class="card" style="width: 20rem; margin:12px">
                    <img src="sports.jpg"card-img-top" alt="...">
                    <div class="card-body">
                      <h5 class="card-title">Not Kishan-Rohit, This Opening Duo No. 1 In IPL 2024: Ex-KKR Star</h5>
                      <p class="card-text">The former Indian cricket team star said that Chennai Super Kings' Devon Conway and Ruturaj Gaikwad can be the second-ranked opening pair in IPL 2024.</p>
                      <a href="https://sports.ndtv.com/ipl-2024/not-ishan-kishan-rohit-sharma-this-opening-duo-can-be-ranked-no-1-in-ipl-2024-ex-kkr-star-5168717" class="btn btn-info">Read More</a>
                      
                    </div>
                  </div>
                  
                  <div class="card" style="width: 20rem; margin:12px">
                    <img src="sports3.jpg"card-img-top" alt="...">
                    <div class="card-body">
                      <h5 class="card-title">Inter Beat Genoa To Take Further Step Towards Serie A Title</h5>
                      <p class="card-text">Juve trail Inter with 11 games of the season remaining after losing 2-1 at Napoli on Sunday.</p>
                      <a href="https://sports.ndtv.com/ipl-2024/not-ishan-kishan-rohit-sharma-this-opening-duo-can-be-ranked-no-1-in-ipl-2024-ex-kkr-star-5168717" class="btn btn-info">Read More</a>
                      
                    </div>
                 </div>
                </div>    
        </div>
        <div class="col-6">
            <div id="carouselExampleIndicators" class="carousel slide">
                <div class="carousel-indicators">
                  <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                  <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
                  <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
                </div>
                <div class="carousel-inner">
                  <div class="carousel-item active">
                    <img src="sports slide 4.jpeg" class="d-block w-100" >
                  </div>
                  <div class="carousel-item">
                    <img src="sports slide 1.jpeg" class="d-block w-100" >
                  </div>
                  <div class="carousel-item">
                    <img src="sports slide 5.jpeg" class="d-block w-100" >
                  </div>
                </div>
                <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
                  <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                  <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
                  <span class="carousel-control-next-icon" aria-hidden="true"></span>
                  <span class="visually-hidden">Next</span>
                </button>
                <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
              </div>
        </div>
    </div>
</body>
</html>
'''

class MyServer(BaseHTTPRequestHandler):
    def do_GET(self):
        print("Get request received...")
        self.send_response(200) 
        self.send_header("content-type", "text/html")       
        self.end_headers()
        self.wfile.write(content.encode())

print("This is my webserver") 
server_address =('',8000)
httpd = HTTPServer(server_address,MyServer)
httpd.serve_forever()
```
## OUTPUT:
![Screenshot 2024-03-27 203947](https://github.com/ramya23000505/simplewebserver/assets/149370791/ca9af1cf-0d95-4164-9c64-5302ac098397)


## RESULT:
The program for implementing simple webserver is executed successfully.
