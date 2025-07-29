# AfroFashion Dataset

## Overview

This dataset contains a rich and culturally diverse collection of African fashion images structured into hierarchical categories and subcategories. Each image is annotated with metadata such as cultural context, regions of popularity, event suitability, fabric type, color, and gender alignment. The goal is to support research and development of AI-powered multimodal fashion retrieval systems, with a focus on African fashion.

## Categories and Subcategories

### Accessories

- Headwrap
- Gele

### Dresses

- Ball Gown
- Corset Dress

### One-Piece Outfits

- Jumpsuit
- Romper

### Outerwear

- Kimono
- Cloak
- Blazer

### Tops

- Corset Top
- Crop Top

### Bottoms

- Wrapper
- Ankara Skirt
- Palazzo Pants
- High Waist Trousers
- Mini Skirt
- Maxi Skirt
- Straight Cut Trousers
- African Print Shorts

### Traditional Wear

- Agbada
- Dashiki
- Boubou
- Kaftan
- Fugu

Each subcategory (e.g., "Agbada") is stored in its own folder and includes a metadata JSON file with the following structure:

```json
{
  "category": "agbada",
  "description": "Traditional flowing robe with wide sleeves, worn across West Africa, especially by Yoruba in Nigeria and other Muslim communities.",
  "regions": ["West Africa", "Nigeria", "Benin", "Togo", "Ghana (Northern)", "Mali", "Senegal"],
  "event": ["Wedding", "Traditional Ceremony", "Religious Ceremony"],
  "style": ["Ceremonial", "Formal"],
  "gender": ["Male"],
  "total_images": 40,
  "images": [
    {
      "filename": "1.jpg",
      "path": "traditional_wear/agbada/1.jpg",
      "description": "Men agbada and kaftan",
      "colors": ["white"],
      "fabric": ["Cashmere", "Wool"],
      "gender": ["Male"]
    },
    ...
  ]
}
```

## Metadata Description

Each image is annotated with the following:

- `filename`: Image file name.
- `path`: Relative path within the dataset directory.
- `description`: A textual description of the outfit.
- `colors`: List of prominent colors in the outfit.
- `fabric`: Common fabrics used.
- `gender`: Intended gender presentation.

Each subcategory metadata also includes:

- `description`: Cultural and stylistic explanation of the outfit.
- `regions`: Where the style is commonly worn.
- `event`: Suitable occasions.
- `style`: General classification (e.g., ceremonial, casual).
- `gender`: Intended gender classification.

## Dataset Usage

This dataset is ideal for fine-tuning multimodal models like CLIP for:

- African fashion recommendation systems
- Contextual retrieval of traditional clothing
- Region-aware cultural recognition in images

## Sources and Attribution

We do not claim ownership of the images. The dataset was compiled from various publicly available online sources including:

- Afrekea
- Jumia
- Pinterest

This dataset is intended for non-commercial research purposes only.

## Licensing

This dataset is distributed for academic and non-commercial research use only. If you intend to use it beyond that, please ensure proper attribution to the original image sources and comply with their respective licenses.

## Contributions

If you'd like to expand this dataset or contribute metadata enrichments, feel free to reach out.

Emmanuel Akpe
emmanuelakpe1@gmail.com
