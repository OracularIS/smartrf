# Additional Information

Smart RF Plus uses the  real estate of the screen to display 
additional data, enhancing the user experience and providing valuable context for warehouse operations.

## What is it?

Smart RF PLUS leverages the extra screen space to show additional information that can assist users in making informed decisions. This feature enhances the utility of the app by presenting relevant data alongside the primary functions.

### Types

- **MOCA Command**
  - Displays results or outputs from MOCA commands directly on the screen. This allows users to see real-time data and responses from the system.

  Example of using CMD to display grid

  ```sql
     [select ordnum, 
        prtnum , 
        schbat 
          from pckwrk_view 
           where wrkref = '<<FORM_ID.FIELD_ID>>'
          group by prtnum, 
          ordnum, 
          schbat 
     ] 
     |
    if (@prtnum = 'PACEMAKER')
    {
        [select count (ordlin) , 
          ordnum , 
          pckqty as ordqty , 
          schbat , 
          prtnum 
             from pckwrk_view 
              where rownum < 99 
               and schbat = **schbat 
               and appqty = '0' 
               group by ordnum,
             pckqty,
             prtnum,
            schbat
        ]
    }


- **URL**
  - Integrates web content by displaying data from specified URLs. This feature can be used to show dynamic information or web-based applications relevant to warehouse operations.

  - Example of using url to display image 
  ```sql 
       SELECT prtnum 
      FROM pckwrk_view 
          WHERE wrkref = '<<FORM_ID.FIELD_ID>>' 
      GROUP BY prtnum 
      |
      IF (**prtnum = 'YOUR ITEM')
        {
         PUBLISH DATA 
       WHERE image_url = 'https://m.media-amazon.com/images/I/    51MJdhzJ5oL._AC_.jpg' 
        }
  
   ```

- **Images**
  - Supports the display of images, which can be useful for visual references such as product photos, diagrams, or instructional images.

### How to mantain Additional information 
 - **Form Information**
   - To manage information displayed on forms, use the Form Information Menu. Here, you can define what additional data should appear across the screen.

    - Navigate to the form information menu  on the smart rf plus.
    - click on the add button from here  

    <img src="./attachments/additional information/Form_info.png" alt="undirectedmenu" style="height: 200px;margin:auto;display:block">

  
    - Simply add the App Version, the relevant Form ID, and input the Title, Type, and Information you want displayed. You can also arrange the display order by setting a Sort Sequence, ensuring that critical data appears in the right place and in the correct order.
 
      <img src="./attachments/additional information/Form_info_dtl.png" alt="undirectedmenu" style="height: 200px;margin:auto;display:block">
  
- **Field Information**
   - The Field Information Menu lets you manage data for individual fields within a form.

   - Navigate to the form information menu  on the smart rf plus.
   - click on the add button from here 

   <img src="./attachments/additional information/Field_infoi.png" alt="undirectedmenu" style="height: 200px;margin:auto;display:block">
   
  - You can choose the Field ID, along with the App Version and Form ID, to link specific information to particular fields. By setting the Title, Type, and Info, as well as the Sort Sequence.

  <img src="./attachments/additional information/Form_info_dtl.png" alt="undirectedmenu" style="height: 200px;margin:auto;display:block">
