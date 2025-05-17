# 3D-modelling

Repository for the class "3D-Modellierung und Georeferenzierung für Archäolog*innen" taught at the University of Basel in the spring semester 2025.
<br>

# IIIF manifests

<br>

# Why a IIIF manifesto and the 3D model need to be deployed somewhere
You need to deploy the 3D model and the IIIF-manifesto, otherwise you will run into so-called **CORS errors**. Such a CORS error (Cross-Origin Resource Sharing) occurs when a web application tries to access resources from a different domain than the one that provided the page. The server likely will not allow this with the result that the browser will block the request for security reasons.
<br>

# How to deploy a 3D model with the help of GitHub Pages

In order to make the final version of the 3D model publicly available you can use GitHub Pages. 
Log in to your GitHub account, or create an account if you haven't one yet.

You need to have the following items ready:
1. 3D model: Export your 3D model from Blender in .glb format. Be aware that if one or more camera(s) and light(s) have been defined in the 3D model in Blender - e.g. to create a special lighting situation - the export of these settings does not happen automatically. Thus, you need to tick the ‘Cameras’ and ‘Punctual lights’ boxes under ‘Include’ on the right-hand side of the Blender export window.
2. IIIF manifesto: my_manifest.json
3. Paradata: paradata documentation in pdf format

Create a GitHub repository `my_repository` where you want to store your 3D models, the iiif-manifests, and the paradata information.


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
https&#8204;://www&#8204;.morphosource.org/uv/uv.html#?manifest=https&#8204;://my_username.github.io/my_repository/iiif-manifests/my_manifest/my_manifest.json
</p>
<br>
This is a working example if you want to check: https://www.morphosource.org/uv/uv.html#?manifest=https://gautschr.github.io/3D-modelling/iiif-manifests/mitreo/mitreo.json)
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
https&#8204;://uv-v4.netlify.app/#?manifest=https&#8204;://my_username.github.io/my_repository/iiif-manifests/my_manifest/my_manifest.json
</p>
<br>
This is a working example if you want to check: https://uv-v4.netlify.app/#?manifest=https://gautschr.github.io/3D-modelling/iiif-manifests/mitreo/mitreo.json
 
