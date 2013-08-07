Referenze
-------------------------------------------------------------------------------

Mappa dei lavori di Faunalia
...............................................................................

.. rst-class:: map thumbnail
.. image:: images/jobs_map.jpg
   :scale: 50 %
   :alt: Faunalia job locations
   :align: left
   :target: http://www2.faunalia.eu/map/lizmap/www/index.php/view/map/?repository=faunalia&project=faunalia_map_it

.. raw:: html

	<?php require_once('/usr/local/src/website_scripts/backend_ufficio.inc'); ?>

I clienti più importanti
...............................................................................
.. raw:: html
	
	<?php 
		$amm = array();
		$uni = array(); 
		$soc = array();
		$org = array();
		getListsOfCommittenti("it", $amm, $uni, $soc, $org);
	?>
	
Amministrazione pubblica
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
.. raw:: html
	
	<?php printListOfCommittenti($amm); ?>

Università e centri di ricerca
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
.. raw:: html
	
	<?php printListOfCommittenti($uni); ?>

Società
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
.. raw:: html
	
	<?php printListOfCommittenti($soc); ?>

Associazioni ed organizzazioni
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
.. raw:: html

	<?php printListOfCommittenti($org); ?>

Corsi e Seminari
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
.. raw:: html
	
	<?php getTableOfLavoriGis(); ?>

Assistenza e sviluppo
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
.. raw:: html
	
	<?php getTableOfLavoriGis(true); ?>

Le pubblicazioni
...............................................................................

.. raw:: html

	<?php printListOfPubblicazioniFreeGis(); ?>