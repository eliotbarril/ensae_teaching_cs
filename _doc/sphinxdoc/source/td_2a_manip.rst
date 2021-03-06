
.. _l-td2a-manip:

========================
Agilité avec les données
========================

Faire du machine learning veut d'abord dire
être capable de manipuler les données comme bon vous semble
et les représenter à l'aide de graphiques.

.. contents::
    :local:

.. |pyecopng| image:: _static/pyeco.png
            :alt: Economie

.. |pystatpng| image:: _static/pystat.png
            :alt: Statistique

------------

Rappels de programmation
========================

|pyecopng|

*Notebooks*

.. toctree::
    :maxdepth: 2

    notebooks/td2_eco_rappels_1a

.. index:: sérialisation, index, dataframe

------------

Matrices et DataFrames - numpy pandas SQL
=========================================

Import/export de données dans un DataFrame,
manipulation selon une logique SQL,
utilité des index,
`lambda function <http://www.diveintopython.net/power_of_introspection/lambda_functions.html>`_,
premiers graphiques,
commandes magiques.

.. contents::
    :local:
    :depth: 1

DataFrame
+++++++++

|pyecopng| |pystatpng|

*Notebooks*

.. toctree::
    :maxdepth: 2

    notebooks/_gs2a_dataframe

*Modules*

* `pandas <http://pandas.pydata.org/>`_

Array, Matrix
+++++++++++++

|pyecopng| |pystatpng|

*Notebooks*

.. toctree::
    :maxdepth: 2

    notebooks/_gs2a_dnumpy

*Lectures*

* `From Python to Numpy <http://www.labri.fr/perso/nrougier/from-python-to-numpy/>`_

*Modules*

* `numpy <http://www.numpy.org/>`_
* `scipy <https://www.scipy.org/>`_

SQL
+++

|pyecopng| |pystatpng|

*Notebooks*

.. toctree::
    :maxdepth: 2

    ext2a/sql_doc
    notebooks/_gs2a_sql

.. _l-visualisation-td2a:

------------

Visualisation
=============

.. contents::
    :local:
    :depth: 1

Graphes
+++++++

|pyecopng| |pystatpng|

Plan

* Présenter `10 plotting libraries at PyData 2016 <http://www.xavierdupre.fr/app/jupytalk/helpsphinx/2016/pydata2016.html>`_.
* Grouper les étudiants par deux
* Considérer un jeu de données
* Chaque groupe essaye une librairie différente
* Insister sur la visualisation de gros jeu de données

Il existe de nombreuses librairies de visualisation réparties en deux grandes familles.
La première produit des images
(`matplotlib <http://www.xavierdupre.fr/app/jupytalk/helpsphinx/notebooks/im_matplotlib.html#immatplotlibrst>`_,
`seaborn <http://www.xavierdupre.fr/app/jupytalk/helpsphinx/notebooks/im_seaborn.html#imseabornrst>`_,
`networkx <http://www.xavierdupre.fr/app/jupytalk/helpsphinx/notebooks/im_networkx.html#imnetworkxrst>`_),
la seconde produit des graphes animés à l'aide de Javascript
(`bokeh <http://www.xavierdupre.fr/app/jupytalk/helpsphinx/notebooks/js_bokeh.html#jsbokehrst>`_,
`bqplot <http://www.xavierdupre.fr/app/jupytalk/helpsphinx/notebooks/im_networkx.html#imnetworkxrst>`_).
Les librairies les plus récentes implémentent les deux modes en cherchant toujours plus
de simplicité. A ce sujet, il faut jeter un coup d'oeil à
`flexx <https://flexx.readthedocs.io/en/stable/>`_. Elles explorent aussi
la visualisation animée de gros jeux de données telle que
`datashader <http://www.xavierdupre.fr/app/jupytalk/helpsphinx/notebooks/big_datashader.html#bigdatashaderrst>`_.

*Notebook sur matplotlib*

.. toctree::
    :maxdepth: 2

    notebooks/_gs2a_visu

* `Graphes classiques métriques pour des modèles de machine learning <http://www.xavierdupre.fr/app/actuariat_python/helpsphinx/notebooks/seance6_graphes_ml_enonce.html>`_
* `Graphes classiques métriques pour des modèles de machine learning - correction <http://www.xavierdupre.fr/app/actuariat_python/helpsphinx/notebooks/seance6_graphes_ml_correction.html>`_

*Notebook sur Javascript*

.. toctree::
    :maxdepth: 2

    ext2a/javascript_doc

* Lire :ref:`Javascript et traitement de données <blog-js-data>`

*Modules*

* `matplotlib <http://matplotlib.org/>`_
* `seaborn <https://github.com/mwaskom/seaborn>`_
* `bokeh <http://bokeh.pydata.org/en/latest/>`_
* `bqplot <https://github.com/bloomberg/bqplot>`_
* :ref:`l-visualisation`

Cartes
++++++

|pyecopng| |pystatpng|

*Notebooks*

* :ref:`td1acenoncesession12rst`
* :ref:`td1acorrectionsession12rst`
* `Evolution d'une population <http://www.xavierdupre.fr/app/actuariat_python/helpsphinx/notebooks/seance4_projection_population_enonce.html>`_
* `Evolution d'une population - correction <http://www.xavierdupre.fr/app/actuariat_python/helpsphinx/notebooks/seance6_graphes_correction.html>`_

*Formats de données*

* :ref:`Système de coordonnées <blog-donnees-carroyees-2016>` (et données carroyées)
* format de cartes
  `shapefiles <https://en.wikipedia.org/wiki/Shapefile>`_,
  `topoJSON <https://en.wikipedia.org/wiki/GeoJSON#TopoJSON>`_,
  `geoJSON <https://en.wikipedia.org/wiki/GeoJSON>`_,
* `Projections sphériques et conversion <http://www.xavierdupre.fr/app/ensae_projects/helpsphinx/notebooks/chsh_geo.html>`_
* conversion de coordonnées en longitude / latitude
* librairies
  `basemap <http://matplotlib.org/basemap/>`_, ...
* sources :
  `DataMaps <http://datamaps.github.io/>`_,
  `Find Data <https://bost.ocks.org/mike/map/#finding-data>`_

*Modules*

* `basemap <http://matplotlib.org/basemap/>`_
* `cartopy <http://scitools.org.uk/cartopy/>`_
* `pyshp <https://pypi.python.org/pypi/pyshp>`_
* `shapely <https://pypi.python.org/pypi/Shapely>`_
* `pyproj <https://pypi.python.org/pypi/pyproj>`_
* `geopy <https://pypi.python.org/pypi/geopy>`_

Graphes classiques
++++++++++++++++++

(*à venir*)

*Lectures*

* `Maximum & Fast readability of multivariate data vs Label <https://medium.com/data-design/maximum-fast-readability-of-multivariate-data-vs-label-c500572c46d1>`_

*Modules*

* `seaborn <https://seaborn.pydata.org/>`_
* `statsmodels <http://www.statsmodels.org/stable/index.html>`_

Visualiser pour comprendre
++++++++++++++++++++++++++

(*à venir*)

*Modules*

* `TensorBoard <https://www.tensorflow.org/versions/r0.12/tutorials/>`_ : c'est un projet qui risque de prendre pas mal d'ampleur.
  Il sert à visualiser les résultats intermédiaires, à comparer, à voir les résultats d'un processus
  de machine learning, en particulier les réseaux de neurones profond. Même `Keras <https://keras.io/callbacks/#tensorboard>`_ s'y met.
  `How to use tensorboard Embedding Projector ? <http://stackoverflow.com/questions/40849116/how-to-use-tensorboard-embedding-projector/42775951>`_
  Exemples `TensorBoard: Embedding Visualization <http://ahogrammer.com/2016/12/01/tensorboard-embedding-visualization/>`_,
  `An Encounter with Google’s TensorFlow <https://esciencegroup.com/2016/01/05/an-encounter-with-googles-tensorflow/>`_,
  `How to plot a ROC curve with Tensorflow and scikit-learn? <http://stackoverflow.com/questions/36939328/how-to-plot-a-roc-curve-with-tensorflow-and-scikit-learn>`_
