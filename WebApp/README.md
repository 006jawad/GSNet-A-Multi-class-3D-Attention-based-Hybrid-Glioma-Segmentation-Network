![Alt Text](extra/BrainTumorSegmentationusingthewebapplication.gif)


## Requirements
The following modules are necessary for running this web application:<br>
- albumentations==1.3.0
- Flask==1.1.1
- imageio==2.22.4
- ipython==8.4.0
- matplotlib==3.5.3
- nibabel==4.0.2
- nilearn==0.9.2
- numpy==1.23.1
- pandas==1.4.3
- Pillow==9.3.0
- scikit_image==0.19.3
- scikit_learn==1.1.2
- scipy==1.9.1
- seaborn==0.12.2
- torch==1.12.1
- tqdm==4.64.1

## Run Locally

Clone the

```bash
  git clone https://github.com/006jawad/GSNet_.git
```

Go to the project directory

```bash
  cd GSNet_/WebApp
```

Install dependencies

```bash
  pip install -r requirements.txt
```

Start the Web App

```bash
  flask run
```
The web-app takes in input as 3D MRI images in the format of ‘.nii’ files. With the input of FLAIR, t1, t1ce, and t2 MRI scans, our web app can produce the corresponding segmentation masks for WT, TC, and ET regions and further save them locally in the ‘.nii’ file format in under 20 seconds.




## License

This software incorporates code from the publicly available repository  [Bootstrap](https://github.com/twbs/bootstrap) as an integral part of the template. Their code is released under the [MIT License](https://github.com/twbs/bootstrap/blob/main/LICENSE).
