# Jeroen Cookbook Data (IM) 📚

This repository contains the raw recipe data extracted from the Lisa professional cookbooks. It serves as the primary source of truth for the Jeroen platform's recipe database.

## 📂 Contents

- **Cookbook JSONs**: `lisa_book1.json` through `lisa_book7.json`.
- **Data Coverage**: 844+ structured recipes.
- **Fields Included**:
  - Name & Category
  - Ingredients & Detailed Instructions
  - Nutritional Macros (KCAL, KHD, VETTEN, EIWITTEN, VEZELS)
  - Serving sizes and Cooking tips

## 🛠 Data Format

The recipes are stored in a structured JSON format. Example:

```json
{
  "Number": 1,
  "Name": "Energy boosting groene smoothie",
  "Category": "Ontbijt",
  "Recipe_Details": [...],
  "Ingredients": [...],
  "Cooking_TIP": null,
  "Persons_Serving": "2",
  "KCAL": "150",
  "KHD": "8",
  "VETTEN": "11",
  "EIWITTEN": "3",
  "VEZELS": null
}
```

## 🔄 Migration

These files are designed to be imported into the MongoDB database using the migration script located in `jeroen_backend/scripts/importRecipes.js`.

## 📜 Usage

This repository is primarily for data storage and extraction purposes. For the live application, use the **Jeroen Backend** API.
