# PaloAPI


Initial Palo setup

** Will need to turn into python scrip and then webpage presentation

Get API Key:
curl -k -X GET "https://192.168.1.1/api/?type=keygen&user=<username>&password=<password>"
API call for log traffic
 curl -k -G 'https://192.168.1.1/api/?&key=<API-KEy>=&type=log&log-type=traffic&query=' --data-urlencode '(receive_time geq '2012/06/22 08:00:00')'
Returns Job-ID, then we call Job-ID to see results
 curl -k 'https://192.168.1.1/api/?&key=<API-KEY>=&type=log&action=get&job-id=<-job-id>'
 
 
 Palo Documentation:
 https://docs.paloaltonetworks.com/pan-os/9-0/pan-os-panorama-api/pan-os-xml-api-request-types/retrieve-logs-api/example-use-the-api-to-retrieve-traffic-logs.html#idd63be533-040c-448a-9a75-3bfc3dce9652
