# https://pcd-viewer.hkustvgd.com/
* Upload pointclouds data into public_datasets/public_statics/pointclouds on NAS
* Access the file on the viewer by an URL: https://pcd-viewer.hkustvgd.com/?url=lion_takanawa
* https://pcd-viewer.hkustvgd.com will show "vol_total" by default

# About

* Potree is a free open-source WebGL based point cloud renderer for large point clouds. It is based on the [TU Wien Scanopy project](https://www.cg.tuwien.ac.at/research/projects/Scanopy/) and research projects [Harvest4D](https://harvest4d.org/), [GCD Doctoral College](https://gcd.tuwien.ac.at/) and [Superhumans](https://www.cg.tuwien.ac.at/research/projects/Superhumans/).
* Newest information and work in progress is usually available on [twitter](https://twitter.com/m_schuetz)
* Contact: Markus Schütz (mschuetz@potree.org)
* References: 
    * [Potree: Rendering Large Point Clouds in Web Browsers](https://www.cg.tuwien.ac.at/research/publications/2016/SCHUETZ-2016-POT/SCHUETZ-2016-POT-thesis.pdf) (2016)
    * [Fast Out-of-Core Octree Generation for Massive Point Clouds](https://www.cg.tuwien.ac.at/research/publications/2020/SCHUETZ-2020-MPC/) (2020)
    
<a href="http://potree.org/wp/demo/" target="_blank"> ![](./docs/images/potree_screens.png) </a>

# Getting Started

### Install on your PC

Install [node.js](http://nodejs.org/)

Install dependencies, as specified in package.json, and create a build in ./build/potree.

```bash
npm install
```

### Run on your PC

Use the `npm start` command to 

* create ./build/potree 
* watch for changes to the source code and automatically create a new build on change
* start a web server at localhost:1234. 

Go to http://localhost:1234/examples/ to test the examples.

### Deploy to a server

* Simply upload the Potree folderm with all your point clouds, the build directory, and your html files to a web server.
* It is not required to install node.js on your webserver. All you need is to host your files online. 

### Convert Point Clouds to Potree Format

Download [PotreeConverter](https://github.com/potree/PotreeConverter) and run it like this:

    ./PotreeConverter.exe C:/pointclouds/data.las -o C:/pointclouds/data_converted

Copy the converted directory into &lt;potreeDirectory&gt;/pointclouds/data_converted. Then, duplicate and rename one of the examples and modify the path in the html file to your own point cloud.

# Downloads

* [Potree](https://github.com/potree/potree/releases)
* [PotreeConverter ](https://github.com/potree/PotreeConverter/releases) - Convert your point cloud to the Potree format.
* [PotreeDesktop ](https://github.com/potree/PotreeDesktop/releases) - Desktop version of Potree. Allows drag&drop of point clouds into the viewer.


# Funding

Potree is funded by a combination of research projects, companies and institutions. 

Research projects who's funding contributes to Potree:

<table>
	<tr>
		<th>Project Name</th>
		<th>Funding Agency</th>
	</tr>
	<tr>
		<td><a href="https://projekte.ffg.at/projekt/3851914">LargeClouds2BIM</a></td>
		<td><a href="https://www.ffg.at/">FFG</a></td>
	</tr>
	<tr>
		<td><a href="https://harvest4d.org/">Harvest4D</a></td>
		<td><a href="https://ec.europa.eu/transport/themes/research/fp7_en">EU 7th Framework Program 323567</a></td>
	</tr>
	<tr>
		<td><a href="https://gcd.tuwien.ac.at/">GCD Doctoral College</a></td>
		<td><a href="https://www.tuwien.at/en/">TU Wien</a></td>
	</tr>
	<tr>
		<td><a href="https://www.cg.tuwien.ac.at/research/projects/Superhumans/">Superhumans</a></td>
		<td><a href="https://www.fwf.ac.at/">FWF</a></td>
	</tr>
</table>

We would like to thank our sponsors for their financial contributions that keep this project up and running!

<table>
	<tr>
		<th>
			Diamond<br>
			€ 15,000+
		</th>
		<td>
			<a href="http://www.ne.ch/autorites/DDTE/SGRF/SITN/Pages/accueil.aspx">
				<img src="docs/sponsors/sitn_logo.png" height="80px"/> &nbsp;
			</a> &nbsp;
			<a href="http://www.synth3d.co">
				<img src="docs/sponsors/synth.png" height="120"/>
			</a> &nbsp;
			<a href="http://www.geocue.com">
				<img src="docs/sponsors/geocue.png" height="120px"/>
			</a> &nbsp;
			<a href="http://rapidlasso.com">
				<img src="./docs/sponsors/rapidlasso_square_256x2561.png" width="150" height="150"/>
			</a> &nbsp;
		</td>
	</tr>
	<tr>
		<th>
			Gold<br>
			€ 10,000+
		</th>
		<td>
			<a href="https://www.bart.gov">
				<img src="docs/sponsors/bart.png" height="100"/>
			</a>
		</td>
	</tr>
	<tr>
		<th>
			Silver<br>
			€ 5,000+
		</th>
		<td>
			<a href="https://www.skyebrowse.com/">
				<img src="docs/sponsors/SkyeBrowse.png" height="60"/> &nbsp;
			</a>
			<a href="https://biology.anu.edu.au/research/facilities/australian-plant-phenomics-facility-anu">
				<img src="docs/sponsors/APPF full logo.png" height="70"/> &nbsp;
			</a>
			<a href="https://www.limit-addict.fr/">
				<img src="docs/sponsors/limitaddict.png" height="45"/>
			</a>
			<a href="http://georepublic.info">
				<img src="docs/sponsors/georepublic.png" height="45"/>
			</a>
		</td>
	</tr>
	<tr>
		<th>
			Bronze<br>
			€ 1,000+
		</th>
		<td>
			<a href="https://www.kkc.co.jp/english/index.html/">
				<img src="docs/sponsors/kokusaikogyo_logo_02.jpg" height="40"/> &nbsp;
			</a>
			<a href="https://www.unstruk.com/">
				<img src="docs/sponsors/unstruk.png" height="33"/> &nbsp;
			</a>
			<a href="http://scanx.com/">
				<img src="docs/sponsors/scanx.jpg" height="33"/> &nbsp;
			</a>
			<a href="https://www.phoenixlidar.com/">
				<img src="docs/sponsors/PhoenixLidar_Logo.jpg" height="45"/> &nbsp;
			</a>
			<a href="https://www.eventart.at/">
				<img src="docs/sponsors/eventart.png" height="55"/> &nbsp;
			</a>
			<a href="https://www.geodelta.com/">
				<img src="docs/sponsors/geodelta.png" height="35"/> &nbsp;
			</a>
			<a href="https://www.e-cassini.fr/">
				<img src="docs/sponsors/e_cassini.jpg" height="70"/> &nbsp;
			</a>
			<a href="https://www.sogelink.fr/">
				<img src="docs/sponsors/SOGELINK_SO-EASY.png" height="40"/> &nbsp;
			</a>
			<b>Data-viewer</b>
			<a href="http://www.helimap.com/">
				<img src="docs/sponsors/helimap.gif" height="60"/> &nbsp;
			</a>
			<a href="http://www.vevey.ch/">
				<img src="docs/sponsors/vevey.png" height="60"/> &nbsp;
			</a>
			<a href="https://www.yverdon-les-bains.ch/">
				<img src="docs/sponsors/Logo-YLB.png" height="60"/> &nbsp;
			</a>
			<a href="http://archpro.lbg.ac.at">
				<img src="docs/sponsors/archpro_EN_small.png" height="60"/> 
			</a> &nbsp;
			<br>
			<a href="http://www.kts.co.jp">
				<img src="docs/sponsors/kts.png" height="32"/> &nbsp;
			</a>
			<a href="http://veesus.com">
				<img src="docs/sponsors/veesus_small.png" height="40"/> &nbsp;
			</a>
			<a href="http://www.sigeom.ch">
				<img src="docs/sponsors/logo_sigeom.png" height="40"/> &nbsp;
			</a>
		</td>
	</tr>
</table>



# Credits

* The multi-res-octree algorithms used by this viewer were developed at the Vienna University of Technology by Michael Wimmer and Claus Scheiblauer as part of the [Scanopy Project](http://www.cg.tuwien.ac.at/research/projects/Scanopy/).
* [Three.js](https://github.com/mrdoob/three.js), the WebGL 3D rendering library on which potree is built.
* [plas.io](http://plas.io/) point cloud viewer. LAS and LAZ support have been taken from the laslaz.js implementation of plas.io. Thanks to [Uday Verma](https://twitter.com/udaykverma) and [Howard Butler](https://twitter.com/howardbutler) for this!
* [Harvest4D](https://harvest4d.org/) Potree currently runs as Master Thesis under the Harvest4D Project
* Christian Boucheny (EDL developer) and Daniel Girardeau-Montaut ([CloudCompare](http://www.danielgm.net/cc/)). The EDL shader was adapted from the CloudCompare source code!
* [Martin Isenburg](http://rapidlasso.com/), [Georepublic](http://georepublic.de/en/),
[Veesus](http://veesus.com/), [Sigeom Sa](http://www.sigeom.ch/), [SITN](http://www.ne.ch/sitn), [LBI ArchPro](http://archpro.lbg.ac.at/),  [Pix4D](http://pix4d.com/) as well as all the contributers to potree and PotreeConverter and many more for their support.

# Bibtex 

```
@article{SCHUETZ-2020-MPC,
	title =      "Fast Out-of-Core Octree Generation for Massive Point Clouds",
	author =     "Markus Schütz and Stefan Ohrhallinger and Michael Wimmer",
	year =       "2020",
	month =      nov,
	journal =    "Computer Graphics Forum",
	volume =     "39",
	number =     "7",
	doi =        "10.1111/cgf.14134",
	pages =      "13",
	publisher =  "John Wiley & Sons, Inc.",
	pages =      "1--13",
	keywords =   "point clouds, point-based rendering, level of detail",
}
```
