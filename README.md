# EX No.3.2. CREATE 3D MODEL FROM ORTHOGRAPHIC PROJECTION
## DATE:21-10-2026
## AIM:
To create a 3D model from given orthographic projection.

## REQUIREMENTS:
1. Autodesk fusion 360
2. Windows 10
3. 16 GB of RAM (integrated graphics recommend 1 GB or more)
4. 2.5 Mbps or faster download; 500 Kbps or faster upload 

## PROCEDURE:
## 1. Start the design

1. Open Fusion 360 and create a **New Design**.
2. In the Browser, expand **Document Settings** and set the units to **mm** if they are not already set.

## 2. Sketch the main side profile

1. Select **Create Sketch**.
2. Select the vertical plane that will show the bracket’s side profile—typically the **XZ plane** or **YZ plane**.
   <img width="1920" height="1028" alt="Screenshot (293)" src="https://github.com/user-attachments/assets/6ff55e65-d7cf-41f0-a718-a7642f2a91ba" />

3. Choose **Rectangle > 2-Point Rectangle**.
4. Draw a rectangle and enter:
   - **Length:** 120 mm
   - **Height:** 60 mm
   - 
5. Choose **Create > Circle > Center Diameter Circle**.
6. <img width="1920" height="1014" alt="Screenshot (329)" src="https://github.com/user-attachments/assets/1ba3eab4-5e0d-4576-b4aa-9e54ba277261" />

7. Draw the circle where the curved portion should be, then enter **220 mm** for its diameter.
   - Position the circle so its arc forms the intended arch. Use dimensions or constraints to locate its center accurately.
8. Choose **Modify > Trim**. Click the unwanted sections of the circle and any extra line segments to remove them.
<img width="1920" height="1014" alt="Screenshot (351)" src="https://github.com/user-attachments/assets/52020883-0d73-4cee-945c-e2f4c94d1a2b" />

9. Inspect the sketch:
    - The outer outline should be continuous.
    - The intended areas to extrude should be shaded as closed profiles.
    - Remove any duplicate or stray segments.
10. Select **Finish Sketch**.
<img width="1920" height="1014" alt="Screenshot (350)" src="https://github.com/user-attachments/assets/2315e3e3-8330-403d-b257-a7c0a91e67d1" />

## 3. Extrude the main profile

1. Select the closed profile or profiles that make up the main body.
2. Press **E** or choose **Create > Extrude**.
3. Enter the required extrusion distance for the bracket’s width.
4. Set **Operation** to **New Body** if this is the first solid feature.
5. Select **OK**.
<img width="1920" height="993" alt="Screenshot (331)" src="https://github.com/user-attachments/assets/a4218e6a-c8bc-45ef-8abf-4a2aa4b16c13" />

## 4. Sketch and extrude the inner rectangular section

1. Rotate the model so the right-side inner face of the curved section is visible.
2. Select that face and choose **Create Sketch**.
3. <img width="1920" height="1007" alt="Screenshot (332)" src="https://github.com/user-attachments/assets/86654b77-ff5f-4605-8bae-c2adbcc732f5" />

4. Choose **Rectangle > 2-Point Rectangle**.
5. Draw the inner rectangle and dimension it:
   - **Length:** 120 mm
   - **Height:** 30 mm
6. Position it to match the opening and inner side shown in your reference.
7. Select **Finish Sketch**.
8. <img width="1920" height="1004" alt="Screenshot (333)" src="https://github.com/user-attachments/assets/8c708292-21c7-4555-9882-674adfcfc666" />

9. Select the new rectangular profile and press **E** for **Extrude**.
10. Enter the required extrusion distance.
11. Set **Operation** to **Join** if it should merge with the existing body, then select **OK**.

## 5. Apply the fillet to shape the curve

1. Choose **Modify > Fillet**.
2. Select the edge or edges that need rounding to form the curved transition.
3. Enter the fillet radius specified by your drawing.
4. Check the preview to confirm the fillet rounds the intended edges without removing the arch or opening.
5. Select **OK**.
<img width="1920" height="1021" alt="Screenshot (334)" src="https://github.com/user-attachments/assets/816f7445-3077-44c3-a0ec-0819b7e0ea18" />

## 6. Cut the right mounting hole

1. Select the top face of the right mounting section.
2. Choose **Create Sketch**.
3. Choose **Create > Circle > Center Diameter Circle**.
4. Place the circle at the required hole center and enter **40 mm** for its diameter.
5. Use dimensions or constraints to position the circle correctly on the mounting section.
6. Select **Finish Sketch**.
 <img width="1920" height="1014" alt="Screenshot (335)" src="https://github.com/user-attachments/assets/a7800690-5579-4487-b817-0965819fc272" />

7. Select the circular profile and press **E** for **Extrude**.
8. Set **Operation** to **Cut**.
9. Set the extent to **Through All** (or use the specified depth if the drawing requires a blind hole).
10. Select **OK**.
<img width="1920" height="1011" alt="Screenshot (336)" src="https://github.com/user-attachments/assets/8ad9db36-317e-49e8-8776-8ebf303305ee" />

## 7. Cut the hole in the curved section

1. Select the top face of the curved section where the smaller hole belongs.
2. Choose **Create Sketch**.
3. Choose **Create > Circle > Center Diameter Circle**.
4. Place the circle at the required location and enter **20 mm** for its diameter.
5. Select **Finish Sketch**.
6. Select the circular profile and choose **Extrude**.
7. Set **Operation** to **Cut** and choose **Through All**, unless a different depth is specified.
8. Select **OK**.
<img width="1920" height="1017" alt="Screenshot (338)" src="https://github.com/user-attachments/assets/000b78a1-24f5-4285-8902-b65bc30206bd" />
<img width="1920" height="1017" alt="Screenshot (339)" src="https://github.com/user-attachments/assets/cb396a49-3db4-4058-83a6-8b97bcc62440" />

## 8. Create the matching left-side features

1. **Create the inner rectangular section:** Sketch a **120 mm × 30 mm** rectangle on the left-side inner face, then extrude it the required distance with **Join** selected.
2. <img width="1920" height="990" alt="Screenshot (342)" src="https://github.com/user-attachments/assets/ced7051c-5f42-4c2f-b5e2-c2565a07babc" />

3. **Round the curved section:** Apply **Fillet** to the corresponding left-side edge or edges, using the same radius as on the right.
4. **Cut the mounting hole:** Sketch a **40 mm diameter** circle on the top face of the left mounting section, position it to match the right hole, then use **Extrude > Cut > Through All**.
<img width="1920" height="997" alt="Screenshot (345)" src="https://github.com/user-attachments/assets/65f391d1-19f0-4662-aeac-ba251c6506bd" />

Check that the left-side features match the right side.
## 9. Check the finished model

1. Rotate the model and inspect it from the top, front, and side.
2. Confirm that:
   - Both mounting holes are cut through the bracket.
   - The two sides match.
   - The arch and inner opening are clear.
   - The fillets are on the intended edges.
   - No sketch profiles or extrusions remain incomplete.
3. Save the design.
<img width="1920" height="1028" alt="Screenshot (352)" src="https://github.com/user-attachments/assets/54f1f7f8-45b4-4429-88ab-d5f01cf4d2a1" />

## 10. Create the drawing

1. Choose **File > New Drawing > From Design** (or **Design > Drawing > From Design**, depending on your Fusion 360 layout).
2. Select the sheet size, units, and drawing standard required for your assignment.
3. Place the base view, then add projected front, side, and isometric views.
4. Add dimensions for the overall size, 120 mm length, 60 mm height, 30 mm inner rectangle, 220 mm circle/arc, and hole diameters of 40 mm and 20 mm.
5. Add any remaining dimensions from your reference, including extrusion thickness, hole locations, and fillet radius.
6. Save the drawing.
<img width="1920" height="1017" alt="Screenshot (354)" src="https://github.com/user-attachments/assets/89d8fd06-bf1a-4fb3-9c7e-645912b53030" />


## INPUT:
![image](https://user-images.githubusercontent.com/113594316/198823540-38a1b79a-1f68-4876-add9-adf59b98b386.png)

## OUTPUT:
<img width="1920" height="1011" alt="Screenshot (353)" src="https://github.com/user-attachments/assets/525f9a6e-7608-4fe9-a9aa-ed3fbb3552b5" />

## RESULT:
Thus, 3D model is created from orthographic projection.



