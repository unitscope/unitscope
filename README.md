# unitscope

<project>
	<CommonSettings>
		<use what="source" for="Configuration">MI-Standart</use>
		<use what="source" for="MetaInformation">MI-Repository</use>
		<use what="source" for="Dependency">MI-Standart</use>
		<use what="rules">MI-Standart</use>
	</CommonSettings>
</project>


CommonSettings
	Use Source Configuration : MI-Standart
	Use Source MetaInformation :  MI-Repository
	Use Source Dependency : Maven(pom.xml)
	Use Rules : MI-Standart
		Use Rules NamingConvention : %Product% Release %Number% %Patch%
		Use Rules Execution : Ansible
	Use Layout Directory : MI-Standart

ExistRelease
	Use Release Meta-Information : Release 1.2.6.mi
NewRelease
	Use Release Meta-Information : Release 1.2.6 Patch2.mi
Require Resource
  Need Library : lib.jar
  Need JMS Queue : jndi/integration/order
  Need WS Endpoint : http://www.webservice.com/endpoint?WSDL
  Need DataSource : jndi/db/database
Fix
	Delete Java Application (API)
Update
Install
  Install Java Application (API)

