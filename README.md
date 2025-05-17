# 3D-modelling

Repository for the class "3D-Modellierung und Georeferenzierung für Archäolog*innen" taught at the University of Basel in the spring semester 2025.
<br>
<br>

# IIIF manifests

There are several ways to create a IIIF manifesto. 

1. If you have some knowledge about IIIF manifests choose a sample IIIF manifesto from the [IIIF GitHub repository](https://github.com/IIIF/3d/tree/main/manifests) and adapt it manually to your needs.
2. Use the newly developed Blender plugin to create a more complex IIIF manifesto.
3. ...
<br>
<br>

# Why a IIIF manifesto and the 3D model need to be deployed somewhere
You need to deploy the 3D model and the IIIF-manifesto, otherwise you will run into so-called **CORS errors**. Such a CORS error (Cross-Origin Resource Sharing) occurs when a web application tries to access resources from a different domain than the one that provided the page. The server likely will not allow this with the result that the browser will block the request for security reasons.
<br>
<br>

# How to deploy a 3D model with the help of GitHub Pages

In order to make the final version of the 3D model publicly available you can use GitHub Pages. GitHub offers one site per GitHub account and organisation for free.
<br>
<br>
Log in to your GitHub account, or first create an account if you haven't one yet.

You need to have the following items ready:
1. 3D model: Export your 3D model from Blender in .glb format. Be aware that if one or more camera(s) and light(s) have been defined in the 3D model in Blender - e.g. to create a special lighting situation - the export of these settings does not happen automatically. Thus, you need to tick the ‘Cameras’ and ‘Punctual lights’ boxes under ‘Include’ on the right-hand side of the Blender export window.
2. IIIF manifesto: my_manifest.json
3. Paradata: paradata documentation in pdf format
4. A thumbnail of your 3D model in .png format named thumb.png

Create a new GitHub repository `my_repository` where you want to store your 3D models, the iiif-manifests, and the paradata information. I suggest to organise the material which will be uploaded into further sub-folders.
<br>
1. create a subfolder `assets`: upload the 3D model `my_model.glb` here
2. create a subfolder `iiif-manifests`: upload the IIIF manifesto `my_manifest.json` and the thumbnail `thumb.png` here. For our class we created further subfolders within this subfolder - one for each person and object.
3. create a subfolder `paradata`: upload the pdf file with the paradata `my_paradata.pdf` here

The next step ist to change the access state of the repository from `private` to `public` in the `Settings` tab. Then in the `Code and automation` section in the `Settings` tab go to `Pages`. In the section `Build and deployment` choose `Deployment from branch`, the branch `main`, the folder `root` and finally click `Save`. This last action causes the GitHub page to be created and to be live at an address which will look like as follows:
<br>
<p align="center">
  https&#8204;://my_username.github.io/my_repository/
</p>
Each time something is changed in the respective repository, a new deployment of the page will be triggered automatically!
<br>
<br>

# Displaying and discovering your 3D model

There are several IIIF compatible viewers offered by institutions and projects which allow to display and discover your 3D model by simply specifying the address of your IIIF manifest in the html address. Here is a (non-extensive) list:
<br>
### **[MorphoSource](https://www.morphosource.org/)** - a 3D repository of Duke University:
To use MorphoSource, simply append the address of your own IIIF manifesto to the following web address section:
<br>
<p align="center">
  https://www.morphosource.org/uv/uv.html#?manifest=
</p>
<br>
Thus, your full address may be as follows: 
<br>
<p align="center">
https&#8204;://www&#8204;.morphosource.org/uv/uv.html#?manifest=https&#8204;://my_username.github.io/my_repository/iiif-manifests/my_manifest.json
</p>
<br>
This is a working example if you want to check: https://www.morphosource.org/uv/uv.html#?manifest=https://gautschr.github.io/3D-modelling/iiif-manifests/mitreo/mitreo.json
<br>
<br>

### **[Universal Viewer:](https://universalviewer.io/)**
To use Universal Viewer, simply append the address of your own IIIF manifesto to the following web address section:
<br>
<p align="center">
  https://uv-v4.netlify.app/#?manifest=
</p>
<br>
Thus, your full address may be as follows:
<br>
<p align="center">
https&#8204;://uv-v4.netlify.app/#?manifest=https&#8204;://my_username.github.io/my_repository/iiif-manifests/my_manifest.json
</p>
<br>
This is a working example if you want to check: https://uv-v4.netlify.app/#?manifest=https://gautschr.github.io/3D-modelling/iiif-manifests/mitreo/mitreo.json
 
