<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>محصولات</title>
    <style>
        .products {
            text-align: right;
            margin: 2rem auto;
            font-family: Arial, sans-serif;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr); /* 3 columns */
            gap: 2.0rem;
            margin-top: 2rem;
        }

        .product-item {
            text-align: center; /* Center-align the content inside the product item */
        }

        .product-item img {
            width: 400px; /* Fixed width for uniformity */
            height: 300px; /* Fixed height for uniformity */
            object-fit: contain; /* Ensures the entire image is visible without cropping */
            background-color: #f9f9f9; /* Optional: Adds a subtle background to fill empty space */
            border: 1px solid #ddd;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .caption {
            margin-top: 0.5rem;
            font-size: 0.9rem;
            color: #555;
            text-align: center; /* Center-align the caption under the image */
        }
    </style>
</head>
<body>
    <div class="products">
        <h1>محصولات</h1>
        <p>به صفحه محصولات ما خوش آمدید. در اینجا می‌توانید ۱۹ محصول برتر ما را مشاهده کنید. هر محصول با توضیحات مختصر ارائه شده است.</p>
        <div class="product-grid">

            <!-- Product List -->
            <script>
                // Product Data
                const products = [
                    { image: "product_1.jpg", description: "جانانی", alt: "محصول ۱" },
                    { image: "product_2.jpg", description: "زیرگلدان گرد", alt: "محصول ۲" },
                    { image: "product_3.jpg", description: "زیرگلدان گرد بارنگُ‌های متنوع", alt: "محصول ۳" },
                    { image: "product_4.jpg", description: "گلدان مستطیل", alt: "محصول ۴" },
                    { image: "product_5.jpg", description: "گلدان چهارگوش", alt: "محصول ۵" },
                    { image: "product_6.jpg", description: "گلدان چهارگوش رنگی", alt: "محصول ۶" },
                    { image: "product_7.jpg", description: "زیرگلدان چهارگوش بارنگُ‌های متنوع", alt: "محصول ۷" },
                    { image: "product_8.jpg", description: "گلدان چهارگوش بارنگُ‌های متنوع", alt: "محصول ۸" },
                    { image: "product_9.jpg", description: "گلدان گرد رنگی", alt: "محصول ۹" },
                    { image: "product_10.jpg", description: "گلدان کهکشان رنگی", alt: "محصول ۱۰" },
                    { image: "product_11.jpg", description: "گلدان لاله", alt: "محصول ۱۱" },
                    { image: "product_12.jpg", description: "گلدان گرد قهوه‌ای", alt: "محصول ۱۲" },
                    { image: "product_13.jpg", description: "گلدان لاله با رنگ زیبا", alt: "محصول ۱۳" },
                    { image: "product_14.jpg", description: "زیر لاله با زیری", alt: "محصول ۱۴" },
                    { image: "product_15.jpg", description: "گلدان چهارگوش با زیری", alt: "محصول ۱۵" },
                    { image: "product_16.jpg", description: "گلدان کهکشان با زیری", alt: "محصول ۱۶" },
                    { image: "product_17.jpg", description: "جانانی کوچک و متوسط", alt: "محصول ۱۷" },
                    { image: "product_18.jpg", description: "گلدان گرد", alt: "محصول ۱۸" },
                    { image: "product_19.jpg", description: "ظرف غذا زنبور عسل", alt: "محصول ۱۹" },
                ];

                // Generate Product Grid
                const productGrid = document.querySelector('.product-grid');
                products.forEach((product, index) => {
                    const productItem = document.createElement('div');
                    productItem.className = 'product-item';
                    productItem.innerHTML = `
                        <img src="/_pages/assets/images/${product.image}" alt="${product.alt}">
                        <p class="caption">محصول ${index + 1}: ${product.description}</p>
                    `;
                    productGrid.appendChild(productItem);
                });
            </script>

        </div>
    </div>
</body>
</html>