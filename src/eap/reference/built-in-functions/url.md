---
locale: en-us
guid: add42ac6-eb89-4448-8b6e-84ceb8a921df
app_type: mobile apps, reactive web apps
---
# URL

## GetBookmarkableURL

Returns the URL of the screen that is currently being processed.  
The URL returned by this function is a complete URL with the format http://server/module/personal_area/screen?param1=value&amp;param2=value...   
Parameters and their values aren't included when parameters are optional and their values aren't set.  

Available in:  

  * Server-side logic: Yes
  * Client-side logic: Yes
  * Database: Function is evaluated before the aggregate is executed.

### Output

Type: Text  

### Examples

```
GetBookmarkableURL() = "http://myserverat.outsystemscloud.com/Customers/EditCustomer.aspx?CustomerId=1"
```

## GetOwnerURLPath

Returns the URL path of the module that owns the element that is being processed. Note that this function does not return the complete URL but only the component containing the location of the resource within the domain and, if applicable, the personal area.  

Available in:  

  * Server-side logic: Yes
  * Client-side logic: Yes
  * Database: Function is evaluated before the aggregate is executed.

### Output

Type: Text  

### Examples

```
GetOwnerURLPath() = "/Customers/"
```