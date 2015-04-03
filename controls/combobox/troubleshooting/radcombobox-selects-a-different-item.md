---
title: RadComboBox Selects a Different Item
page_title: RadComboBox Selects a Different Item | UI for ASP.NET AJAX Documentation
description: RadComboBox Selects a Different Item
slug: combobox/troubleshooting/radcombobox-selects-a-different-item
tags: radcombobox,selects,a,different,item
published: True
position: 10
---

# RadComboBox Selects a Different Item



## 

__DESCRIPTION__

The user selects an Item from the drop down.

__PROBLEM__

Another item gets selected.

__CAUSE__

Items have identical values. On blur or postback the RadComboBox searches for the first Item with the selected value and selects it.

````ASPNET
	    <telerik:RadComboBox ID="RadComboBox1" runat="server">
	       <Items>
	           <telerik:RadComboBoxItem Text="Item 1" Value="1" />
	           <telerik:RadComboBoxItem Text="Item 2" Value="1" />
	           <telerik:RadComboBoxItem Text="Item 3" Value="1" />
	       </Items>
	    </telerik:RadComboBox> 
````



The same behavior will manifest when the items are having the same Text and no Values:

````ASPNET
	    <telerik:RadComboBox ID="RadComboBox1" runat="server">
	       <Items>
	           <telerik:RadComboBoxItem Text="Item" />
	           <telerik:RadComboBoxItem Text="Item" />
	           <telerik:RadComboBoxItem Text="Item" />
	       </Items>
	    </telerik:RadComboBox> 
````



__RESOLUTION__

Make sure that all Items have __unique__ values.