=======
History
=======

0.1.3 (2019-11-21)
------------------
Fixed a bug where networkType used to be a string, now it is a list of strings and we specify 'list_of_string'
type when setting networkType attribute with network.set_network_attribute("networkType", networkType, 'list_of_string').
This results in correct representation of networkType in CX model, for example:
{"n":"networkType","v":["interactome","ppi"],"d":"list_of_string"}.

0.1.2 (2019-10-25)
------------------
In organism_load_plan.json, changed types of edge columns
"Experimental System Type" and "Throughput" to be "list_of_string",
and "Score" to be "list_of_double".
This change resolves UD-761 Biogrid network can't be imported to Cytoscape.

0.1.1 (2019-08-23)
------------------
* First release on PyPI.
