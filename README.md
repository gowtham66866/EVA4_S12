# EVA4_S12

TinyImageNet - ResNet18

Objective

To Train Resnet18 on Tiny ImageNet dataset

Epoch - 50

Accuracy expected - 50%+

Result

Accuracy achieved - 60.82%

Accuracy vs Learning Rate

![image](https://user-images.githubusercontent.com/36323558/85954363-853eb880-b994-11ea-8393-ad481e6a2789.png)

Train and Test Accuracy
![image](https://user-images.githubusercontent.com/36323558/85954395-adc6b280-b994-11ea-968f-674017fe9ce8.png)

Misclassified Images
![image](https://user-images.githubusercontent.com/36323558/85954455-24fc4680-b995-11ea-8cd8-09d04295e314.png)

GradCam Output
![image](https://user-images.githubusercontent.com/36323558/85954468-537a2180-b995-11ea-928e-5bc349a83fb4.png)

Annotation

Objective

To download 50 images of dog and annotate them with bounding boxes around dogs

Find best number of clusters

Best number of clusters - 3
![image](https://user-images.githubusercontent.com/36323558/85954509-9b00ad80-b995-11ea-98ee-4bc8430459b9.png)

JSON Explained 
    "info": {    ===> Meta data about the VGG Annotator 
    
        "year": 2020,
        
        "version": "1.0",
        
        "description": "VIA project exported to COCO format using VGG Image Annotator (http://www.robots.ox.ac.uk/~vgg/software/via/)",
        
        "contributor": "",
        
        "url": "http://www.robots.ox.ac.uk/~vgg/software/via/",
        
        "date_created": "Fri Jun 26 2020 07:47:58 GMT+0530 (India Standard Time)"
        
    },
    
    "images": [    ==> Array of images with meta information
    
      {
      
            "id": 1,    ==> Unique Id of the image
            
            "width": 660,  ==> Width of the image
            
            "height": 919,  ==> Height of the image 
            
            "file_name": "1.jpeg",  ==> File name of the image
            
            "license": 0,     
            
            "date_captured": ""
            
        }
        ],
    "annotations": [{     ==> Array of annotation information
    
            "segmentation": [ ==> Defines four corners coordinates of the bounding box
            
                [
                
                    48,      ==> x1 (x coordinate of top-left corner)
                    
                    2,       ==> y1 (y coordinate of top-left corner)
                    
                    305,     ==> x2 (x coordinate of top-right corner   x2 = x1 + width of bbox = 48+257 = 305)
                    
                    2,       ==> y1 (y coordinate of top-right corner)
                    
                    305,     ==> x2 (x coordinate of bottom-right corner)
                    
                    159,     ==> y2 (x coordinate of bottom-right corner  y2 = y1 + height of bbox = 2+157 = 159)
                    
                    48,      ==> x1 (x coordinate of bottom-left corner)
                    
                    159      ==> y2 (x coordinate of bottom-left corner)
                    
                ]
                
            ],
            
            "area": 40349,   ==> Area of bbox = height*width = 257*157 = 40349
            
            "bbox": [   ==> Bounding box details
            
                48,          ==> x coordinate of Top-left corner
                
                2,           ==> y coordinate of Top-left corner
                
                257,         ==> Width of the bounding box
                
                157          ==> Height of the bounding box
                
            ],
            
            "iscrowd": 0,
            
            "id": 1,          ==> Unique id of Annotation
            
            "image_id": 48,   ==> Image's unique id
            
            "category_id": 1  ==> Class Id to which this object belongs to
            
        }],
        
    "licenses": [   ==> License information
    
        {
        
            "id": 0,
            
            "name": "Unknown License",
            
            "url": ""
            
        }
        
    ],
    
    "categories": [   ===> Annotation meta
    
        {
        
            "supercategory": "class",   ==> "class" information
            
            "id": 1,                    ==> Unique Id of this class
            
            "name": "DOG"               ==> Name of the class
            
        },
        
        {
        
            "supercategory": "class",  ==> "class" information
            
            "id": 2,                   ==> Unique Id of this class
            
            "name": "CAT"              ==> Name of the class
            
        },
        
        {
        
            "supercategory": "class", ==> "class" information
            
            "id": 3,                  ==> Unique Id of this class
            
            "name": "HUMAN"           ==> Name of the class
            
        }
        
    ]
    
}




