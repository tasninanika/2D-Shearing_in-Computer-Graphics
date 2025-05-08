# 2D Shearing in Computer Graphics

## 📌 Description

2D Shearing is a geometric transformation used in computer graphics to slant the shape of an object. It distorts the object along the X-axis or Y-axis, depending on the shearing factors applied.

Shearing does not affect the size of the object but changes its shape. It is particularly useful in animation, modeling, and creating effects like italic text or simulating motion blur.

There are two types of shearing in 2D:
- **X-shear:** Moves points horizontally, depending on their y-coordinate  
  → `x' = x + shx * y`, `y' = y`
- **Y-shear:** Moves points vertically, depending on their x-coordinate  
  → `x' = x`, `y' = y + shy * x`

You can also combine both for a diagonal slant.

---

## 🧮 Algorithm: 2D Shearing of a Square

**Step 1:** Define the original square points in (x, y) format.

**Step 2:** Define shearing factors:
- `shx` for X-shear (horizontal slant)
- `shy` for Y-shear (vertical slant)

**Step 3:** For each point `(x, y)` in the original square:
- Compute new coordinates:
  - `x' = x + shx * y`
  - `y' = y + shy * x`
- Store `(x', y')` in a new list.

**Step 4:** Append the first point at the end of both lists to visually close the square.

**Step 5:** Separate x and y coordinates from:
- Original square
- Sheared square

**Step 6:** Use `matplotlib` to plot both shapes:
- Original square in one color
- Sheared square in another

**Step 7:** Add axis, grid, labels, title, and legend for better visualization.

---

## 🖼 Output

The graph displays:
- Original square (green)
- Sheared square (cyan) slanted based on the chosen shearing factor.

---

## 🛠 Technologies Used

- Python
- Matplotlib
