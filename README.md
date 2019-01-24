# TA-osquery
An Splunk technology add-on for osquery

# Features
* Parses and extracts fields for the following logs: 
	* `osqueryd.INFO, osqueryd.WARNING, osqueryd.ERROR`
	* `osqueryd.results.log`
	* `osqueryd.snapshots.,log`
* Provides Datamodel Mapping for:
	* **Alerts** Data Model base on alerts from packs
	* **Changess** Data Model base on FIM events from packs
	* **Endpoint** Data Model base on Splunks Query Pack (todo)
* Does _correct_ time extraction 

# Deploying
1. Remember to drop the TA in your indexers as well as your forwarded
2. Do not forget to remove the example `default/inputs.conf`
3. Add the Splunk query pack to your osquery agent (todo)

# To Do's
* Test Alert Data model mapping for Alerts in the results log
* Test Changes Data model mapping for FIM events in the results log
* Create a splunk query pack
* Populate Endpoint DM with the results of the splunk query pack

