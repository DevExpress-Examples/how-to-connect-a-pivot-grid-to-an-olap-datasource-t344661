<!-- default file list -->
*Files to look at*:

* [MainWindow.xaml.cs](./CS/WpfOlapRetrieveFieldsExample/MainWindow.xaml.cs) (VB: [MainWindow.xaml.vb](./VB/WpfOlapRetrieveFieldsExample/MainWindow.xaml.vb))
<!-- default file list end -->
# How to connect a Pivot Grid to an OLAP datasource


If you have a cube on the OLAP server (Microsoft Analysis Services), you can view its data using the <a href="https://documentation.devexpress.com/WPF/CustomDocument7228.aspx">Pivot Grid</a>. In this example, you will see how to specify connection settings to the server and create fields that represents specific measures and dimensions of the cube.<br><br>To bind the Pivot Grid control to an OLAP cube, follow the steps below.<br><br>1. Set <em>ADOMD</em> as a data provider using the <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfPivotGridPivotGridControl_OlapDataProvidertopic">PivotGridControl.OlapDataProvider</a> property.<br>2. Specify connection settings to the server using the <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfPivotGridPivotGridControl_OlapConnectionStringtopic">PivotGridControl.OlapConnectionString</a> property. The connection string used in the example is shown below.<br><em>OlapConnectionString="Provider=MSOLAP;Data Source=<a href="http://demos.devexpress.com/Services/OLAP/msmdpump.dll;Initial">http://demos.devexpress.com/Services/OLAP/msmdpump.dll;Initial</a> catalog=Adventure Works DW Standard Edition;Cube name=Adventure Works;Query Timeout=100;"</em><br>3. Create fields for all the measures and dimension in the bound OLAP cube, and moves these fields to the specified area, making them hidden. To do it, use the <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfPivotGridPivotGridControl_RetrieveFieldstopic(vUYR8Q)">PivotGridControl.RetrieveFields</a> method overload and set the field's visibility to <strong>false</strong>.<br>4. Place some of the created fields within corresponding Pivot Grid Control areas and set the visibility of the fields to <strong>true </strong>using the <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfPivotGridPivotGridField_Visibletopic">PivotGridField.Visible</a> property.<br><br>Use the invoked <a href="https://documentation.devexpress.com/#WPF/CustomDocument8018">Customization Form</a> to specify the Pivot Grid control's layout.<br><br>To learn more about OLAP Datasources, see <a href="https://documentation.devexpress.com/#WPF/CustomDocument11782">OLAP Datasources</a>.

<br/>


