# filesystem

filesystem object

  


This function returns the create time of a file.

# datetime get_create_date_time(string path)

## Parameters

variable| description  
---|---  
path | The path of the file.  
  
## Return Value

The datetime object with the set date of the created date and time of the file on success, a runtime error on failure.

## Remarks

Be warned when using this function. Make sure the file exists. Failing to retrieve the created date and time will result in a runtime error being triggered.

## Example
    
    
    void main()
    {
    filesystem f;
    datetime test = f.get_create_date_time("test.ngt");
    // The datetime object (test) now has the date that the test.ngt file was created.
    }
    
