


# lib_Kafka

# This is a the Kafaka connector for Convertigo.

The connector will allow Convertigo applications to produce Kafka messages on topics

## Symbols

| Name                  | Default Value |  Usage                                 |
|-----------------------|---------------|----------------------------------------|
|lib_Kafka.server_port  |localhost:19092|The host and port of the kafka broker   |
|-----------------------|---------------|----------------------------------------|




For more technical informations : [documentation](./project.md)

- [Installation](#installation)
- [Sequences](#sequences)
    - [Producer](#producer)


## Installation

1. In your Convertigo Studio click on ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/icons/studio/project_import.gif?raw=true "Import a project in treeview") to import a project in the treeview
2. In the import wizard

   ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/tomcat/webapps/convertigo/templates/ftl/project_import_wzd.png?raw=true "Import Project")
   
   paste the text below into the `Project remote URL` field:
   <table>
     <tr><td>Usage</td><td>Click the copy button at the end of the line</td></tr>
     <tr><td>To contribute</td><td>

     ```
     lib_Kafka=/Users/olivierpicciotto/wrks/lib_Kafka/.git:branch=master
     ```
     </td></tr>
     <tr><td>To simply use</td><td>

     ```
     lib_Kafka=/Users/olivierpicciotto/wrks/lib_Kafka//archive/master.zip
     ```
     </td></tr>
    </table>
3. Click the `Finish` button. This will automatically import the __lib_Kafka__ project


## Sequences

### Producer

Produce a record with a key and a message on a topic. Will return the produced offset and the partition

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>message</td><td>The message data to be produced , this can be a JSON string</td>
</tr>
<tr>
<td>topic</td><td>the topic where the message as to be produced</td>
</tr>
</table>


