# 3D-modelling

Repository for the class "3D-Modellierung und Georeferenzierung für Archäolog*innen" taught at the University of Basel in the spring semester 2025.

# IIIF manifests


# How to deploy a 3D model with the help of GitHub Pages

In order to make the final version of the 3D model publicly available you can use GitHub Pages. 
Log in to your GitHub account, or create an account if you haven't one yet.

You need to have the following items ready:
1. 3D model: Export your 3D model from Blender in .glb format. Be aware that if one or more camera(s) and light(s) have been defined in the 3D model in Blender - e.g. to create a special lighting situation - the export of these settings does not happen automatically. Thus, you need to tick the ‘Cameras’ and ‘Punctual lights’ boxes under ‘Include’ on the right-hand side of the Blender export window.
2. IIIF manifest: my_manifest.json
3. Paradata: paradata documentation in pdf format

Create a GitHub repository

# Displaying and discovering your 3D model

<p>There are several IIIF compatible viewers offered by institutions and projects which allow to display and discover your 3D model by simply specifying the address of your IIIF manifest in the html address. Here is a (non-extensive) list: </p>
<br>
<h2>[MorphoSource](https://www.morphosource.org/) - a 3D repository of Duke University:</h2>
<br>
To use MorphoSource, simply append the address of your own IIIF manifest to the following web address section:
<br>
[https://www.morphosource.org/uv/uv.html#?manifest=](https://www.morphosource.org/uv/uv.html#?manifest=)
<br>
Thus, your full address may be as follows: 
<br>
[https://www.morphosource.org/uv/uv.html#?manifest=https://username.github.io/my_repository/iiif-manifests/my_manifest/my_manifest.json](https://www.morphosource.org/uv/uv.html#?manifest=https://username.github.io/my_repository/iiif-manifests/my_manifest/my_manifest.json)
<br>
[Here](https://www.morphosource.org/uv/uv.html#?manifest=https://gautschr.github.io/3D-modelling/iiif-manifests/mitreo/mitreo.json) is a working example if you want to check.

<h2>[Universal Viewer:](https://universalviewer.io/)</h2>
<br>
To use Universal Viewer, simply append the address of your own IIIF manifest to the following web address section:
<br>
[https://uv-v4.netlify.app/#?manifest=](https://uv-v4.netlify.app/#?manifest=)
<br>
Thus, your full address may be as follows:
<br>
[https://uv-v4.netlify.app/#?manifest=https://username.github.io/my_repository/iiif-manifests/my_manifest/my_manifest.json](https://uv-v4.netlify.app/#?manifest=https://username.github.io/my_repository/iiif-manifests/my_manifest/my_manifest.json)
<br>
[Here](https://uv-v4.netlify.app/#?manifest=https://gautschr.github.io/3D-modelling/iiif-manifests/mitreo/mitreo.json) is a working example if you want to check.
 
