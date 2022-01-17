# fiap-aso-grupo26

oc new-project mbaaso-grupo26

oc create -f imagestream.yml

oc create -f buildconfig.yml

oc create -f deploymentconfig.yml

oc create -f hpa.yml

oc create -f service.yml

oc create -f route.yml




