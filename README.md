# camunda.common.jsf.components

This could be some reusable JSF Components to be used in conjunction with camundas process diagrams.

To get started install this project with maven
```maven
mvn clean install
```

Now go to https://github.com/zerounix/camunda.common.jsf.components.example and clone this project.

Next thing is fire up your camunda engine with invoice demo preinstalled (just download a vanilla camunda distributation
package and fire up start-camunda.bat/sh).

Now package the example and deploy it. You can now point your browser to http://localhost:8080/amunda.common.jsf.components.example

It's that simple:

The JSF Example application includes the custom JSF Component from the first jar in the page:

```java
<html lang="de" xmlns="http://www.w3.org/1999/xhtml" 
  ....
	xmlns:bpmn="http://java.sun.com/jsf/composite/bpmn">
```

and then uses the diagram tag:

```java
<bpmn:diagram taskId="a_task_id" engine="a_process_engine" restenginePath="url_to_camundas_restengine" /> 
```

Can displaying process diagrams get simpler?
