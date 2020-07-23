## Cracks and Potholes in Road Images Dataset

### Abstract 

The poor condition of the roads directly affects traffic safety. In several countries, vehicles that survey road information are already used. These vehicles capture information and images that are used to define highway intervention and maintenance strategies. The images captured by these vehicles allow the identification of problems found on the highways, however in many cases they need manual analysis by trained technicians. 

Defects such as cracks and potholes can be identified automatically using image processing and machine learning techniques. Developed researches in the field of machine learning requires a large set of images, whether for training the algorithms or during the recognition test. In this context, this dataset was created containing images of defects in asphalted roads in Brazil, in order to be used for a study on the detection of cracks and potholes in asphalted roads, using texture descriptors and machine learning algorithms such as Support Vector Machine, K-Nearest Neighbors and Multi-Layer Perceptron Neural Network. 

The dataset was developed using images made available by Brazilian National Department of Transport Infrastructure (NDTI), through the Access to Information Law - Protocol 50650.003556/2017-28. The images are from highways in the states of Espírito Santo, Rio Grande do Sul and the Federal District. 2235 images were selected manually, following criteria such as not showing signs of vehicles and people, as well as not having image defects. This work consists of 2235 samples of roads where each image has 3 masks that delimit the vehicle's path and crack and pothole defects.

### Keywords

Road, Pavement, Defects, Detection, Recognition, Crack, Pothole

### Authors

Bianka Tallita Passos, Mateus Junior Cassaniga, Anita Maria da Rocha Fernandes, Kátya Balvedi Medeiros, Eros Comunello

### Affiliations

University of Itajaí Valley – UNIVALI. Santa Catarina – Brazil.

### Value of Data

- The data can be used to train classifiers or artificial neural networks to identify a lane, cracks or potholes. Different classifiers can be trained to identify the best type of image for a given problem, such as defects recognition for road maintenance.
- The federal road network in several countries is monitored using vehicles that capture images. However, the analysis and marking of the defects found in these images is done posteriori, by technicians in laboratories. A tool capable to detect and classify defects in these images in an automated way could replace this step, speeding up the process and reducing the final cost of monitoring.
- Vision-based methods, which use image processing to detect defects in the floor, enables a low investment cost and can be achieved with common cameras.
- Cracks and potholes are types of defects in the pavements that can compromise the safety and quality of the roads. The identification of such defects is an important step for intervention and maintenance strategies to be carried out.

### Data Description

The dataset images were extracted from videos captured by NDTI, using a Highway Diagnostic Vehicle (HDV). To register the highways, the HDV is equipped with a high-resolution camera and two cameras for filming.

The camera is installed on the highest part of the vehicle, facing the front and with an inclination closer to orthogonality. Thus, the visibility of the pavement is 15 meters. This camera captures images with a minimum resolution of 4 megapixels, every 5 meters away [1].

The video cameras, installed on the front and rear of the HDV, are responsible for the continuous capture of videos with a rate of 30 Frames Per Second (FPS). The resolution is at least 1280x729 and respects the 16:9 aspect ratio. Figure 1 shows the main characteristics of the
HDV [1].

![](/figures/1.png)
Figure 1. Representation of the HDV used by NDTI [1]: (a) satellite tracking system (b) high-resolution camera (c) recording cameras (d), precision odometer and (e) laser sensors.

The images were provided by the NDTI on a hard disk, and with the following characteristics:
- The images were captured between 2014 and 2017; and
- They are images from highways of Espírito Santo state (BR 101, 259, 262, 393, 447, 482 and 484), Rio Grande do Sul state (BR 101, 290 and 386) and Federal District (BR 010, 020, 060, 070, 080 and 251).

The dataset was developed using only the images provided by NDTI. A total of 2235 images were selected manually, considering the following criteria:
1. To count as an image with damaged asphalt, present crack(s) and/or pothole(s);
2. Do not contain vehicles in images;
3. Do not contain people in images; and
4. No problems due to capture, such as defects in colors (colors that do not correspond to the rest of the image) and defects in the image (such as missing parts).

Figure 2 shows some images present in this database.

![](/figures/2.png)

Figure 2. Example of some images from the dataset.

Each image has 3 masks - binary images in PNG (Portable Network Graphics) format - separated for each type of annotation: road, crack and pothole. The annotation of the road consisted of demarcating the total region corresponding to the vehicle's road, as shown in Figure 3.

![](/figures/3.png)

Figure 3. Road region annotation example.

The annotation of cracks and potholes consisted of the defect selection, maintaining its shape as much as possible, as shown in Figure 4. 

![](/figures/4.png)

Figure 4. Pothole annotation example (blue) and cracks (red).

Figure 5 shows the separate masks for each type of annotation - road, pothole and crack - that compose this dataset.

![](/figures/5.png)

Figure 5. Example of the original image (a) and the masks corresponding to the road region (b), pothole (c) and crack (d).

For the identification of cracks and potholes, the same definitions presented in NDTI [2] and Fernandes, Oda and Zerbini [3] were used.

### Experimental Design, Materials and Methods

The images provided by NDTI have no labelling or any information referring to the damage present on the roads. A tool was developed that made it possible to annotate these objects/defects in order to create the ground-truth available in this article. The tool received as input the original image, where it is possible to select the region of the road and the defects found. As a result, the marks generated were converted into masks.

### Acknowledgments

This study was financed in part by the Coordenação de Aperfeiçoamento de Pessoal de Nı́vel Superior – Brasil (Higher Level Personnel Improvement Coordination - Brazil - CAPES) - Finance Code 001.

### References

[1] Brazil. Departamento Nacional de Infra-Estrutura de Transportes (National Department of Transport Infraestructure) . Edital Pregão Eletrônico No 0268/16-00, 2016.

[2] NDTI. Norma DNIT 005/2003 - TER: Defeitos nos pavimentos flexíveis e semi-rígidos. Rio de Janeiro. 2003.

[3] Fernandes Jr, J. L.; Oda, S.; Zerbini, L. F. Defeitos e atividades de manutenção e reabilitação em pavimentos asfálticos. Universidade de São Paulo: Escola de Engenharia de São Carlos. São Paulo (SP), 1999.

### DOI

10.17632/t576ydh9v8.4

### Cite this dataset

[Passos, Bianka T.; Cassaniga, Mateus J.; Fernandes, Anita M. R. ; Medeiros, Kátya B. ; Comunello, Eros (2020), “Cracks and Potholes in Road Images”, Mendeley Data, V4, doi:10.17632/t576ydh9v8.4](http://dx.doi.org/10.17632/t576ydh9v8.4) 

### Corresponding author(s)

[Bianka Passos](mailto:biankatpas@gmail.com)

### Download
[Mendeley Data](
https://data.mendeley.com/datasets/t576ydh9v8/3/files/afc7c028-06e0-475b-b190-e008df681b19/Cracks-and-Potholes-in-Road-Images.zip?dl=1
)
