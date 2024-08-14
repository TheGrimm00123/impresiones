<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="viewport" content="width=device-width, initial-scale=1.0">
    <title>Impresión de Imágenes</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="icon" type="image/png" sizes="16x16" href="https://www.kleur.co/wp-content/uploads/2017/02/DIFERENCIAS-IMPRESION-DIGITAL-IMPRESION-OFFSET.png">

    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f4f4f9;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: flex-start;
            min-height: 100vh;
        }

        .main-container {
            display: flex;
            gap: 20px;
            align-items: flex-start;
            width: 100%;
        }

        .container {
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            width: 300px;
            text-align: center;
            position: sticky;
            top: 20px;
            left: 0;
        }

        h1 {
            text-align: center;
            color: #444;
            margin-bottom: 20px;
        }

        #error-message {
            color: red;
            text-align: center;
            margin-top: 10px;
            display: none;
        }

        #preview-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            width: calc(100% - 320px);
            margin-left: auto;
            max-height: 800px;
            overflow-y: auto;
        }

        #preview {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 20px;
            width: 100%;
        }

        .page {
            margin-bottom: 20px;
            display: grid;
            gap: 5px;
            background-color: #fff;
            padding: 10px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            border: 1px solid #ddd;
            box-sizing: border-box;
            width: 100%;
        }

        .preview-image {
            border: 1px solid #ccc;
            border-radius: 4px;
            overflow: hidden;
            box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .preview-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .form-group {
            margin-bottom: 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        label {
            margin-right: 10px;
            font-weight: bold;
        }

        input[type="file"] {
            margin-top: 10px;
        }

        select, input[type="checkbox"], input[type="number"], button {
            padding: 8px;
            border-radius: 4px;
            border: 1px solid #ccc;
            font-size: 14px;
        }

        button {
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #45a049;
        }

        button:active {
            background-color: #3e8e41;
        }

        #printButton {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 16px;
        }

        #customSizeOptions {
            display: none;
            margin-top: 20px;
        }

        #pagination {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-top: 20px;
        }

        .page-navigation {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 4px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .page-navigation:disabled {
            background-color: #ccc;
            cursor: not-allowed;
        }

    </style>
</head>
<body>
    <div class="main-container">
        <div class="container">
            <h1>Impresión de Imágenes</h1>
            <input type="file" id="imageUpload" multiple accept="image/*">
    
            <!-- Sección original de selección de imágenes por hoja -->
            <div class="form-group">
                <label for="imagesPerPage">Imágenes por hoja:</label>
                <select id="imagesPerPage">
                    <option value="1">1</option>
                    <option value="2">2</option>
                    <option value="3">3</option>
                    <option value="4">4</option>
                    <option value="6">6</option>
                    <option value="9">9</option>
                    <option value="12">12</option>
                    <option value="16">16</option>
                    <option value="20">20</option>
                    <option value="25">25</option>
                    <option value="30">30</option>
                    <option value="35">35</option>
                    <option value="40">40</option>
                </select>
            </div>
            <div class="form-group">
                <label for="paperSize">Tamaño del papel:</label>
                <select id="paperSize">
                    <option value="letter">Carta (8.5" x 11")</option>
                    <option value="a4">A4 (210mm x 297mm)</option>
                    <option value="legal">Oficio (8.5" x 13")</option>
                </select>
            </div>
            <div class="form-group">
                <label for="orientation">Orientación:</label>
                <select id="orientation">
                    <option value="portrait">Vertical</option>
                    <option value="landscape">Horizontal</option>
                </select>
            </div>
            <div class="form-group">
                <label for="fillImage">Rellenar imagen:</label>
                <input type="checkbox" id="fillImage" checked>
            </div>
            <div class="form-group">
                <label for="stretchImage">Estirar imagen:</label>
                <input type="checkbox" id="stretchImage" checked>
            </div>
    
            <!-- Checkbox para habilitar tamaño personalizado -->
            <div class="form-group">
                <label for="useCustomSize">Usar tamaño personalizado:</label>
                <input type="checkbox" id="useCustomSize" onclick="toggleCustomSize()">
            </div>
    
            <!-- Nueva sección de especificación de tamaño de imagen, inicialmente oculta -->
            <div id="customSizeOptions">
                <h2>Especificar Tamaño de Imagen</h2>
                <div class="form-group">
                    <label for="imageWidth">Ancho de imagen (cm):</label>
                    <input type="number" id="imageWidth" value="5" min="1" disabled>
                </div>
                <div class="form-group">
                    <label for="imageHeight">Alto de imagen (cm):</label>
                    <input type="number" id="imageHeight" value="5" min="1" disabled>
                </div>
            </div>
            
            <button onclick="generatePreview()">Generar Vista Previa</button>
            <div id="error-message">Por favor, selecciona al menos una imagen.</div>
            <button id="printButton" onclick="printImages()">Imprimir</button>
        </div>

        <div id="preview-container">
            <h2>Vista Previa</h2>
            <div id="preview"></div>
            <div id="pagination">
                <button id="prevPage" class="page-navigation" onclick="changePage(-1)" disabled>Anterior</button>
                <button id="nextPage" class="page-navigation" onclick="changePage(1)" disabled>Siguiente</button>
            </div>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>

<script>
const imageUpload = document.getElementById('imageUpload');
const imagesPerPageSelect = document.getElementById('imagesPerPage');
const imageWidthInput = document.getElementById('imageWidth');
const imageHeightInput = document.getElementById('imageHeight');
const useCustomSizeCheckbox = document.getElementById('useCustomSize');
const paperSizeSelect = document.getElementById('paperSize');
const orientationSelect = document.getElementById('orientation');
const fillImageCheckbox = document.getElementById('fillImage');
const stretchImageCheckbox = document.getElementById('stretchImage');
const preview = document.getElementById('preview');
const errorMessage = document.getElementById('error-message');
const customSizeOptions = document.getElementById('customSizeOptions');

let currentPageIndex = 0;
let totalPages = 0;
let pages = [];

function toggleCustomSize() {
    const useCustomSize = useCustomSizeCheckbox.checked;
    imageWidthInput.disabled = !useCustomSize;
    imageHeightInput.disabled = !useCustomSize;
    customSizeOptions.style.display = useCustomSize ? 'block' : 'none';
}

function getPaperDimensions() {
    const paperSize = paperSizeSelect.value;
    const orientation = orientationSelect.value;
    let width, height;

    if (paperSize === 'letter') {
        width = 800; // Carta (8.5" x 11")
        height = 1100;
    } else if (paperSize === 'a4') {
        width = 793; // A4 (210mm x 297mm)
        height = 1122;
    } else if (paperSize === 'legal') {
        width = 800; // Oficio (8.5" x 13")
        height = 1300;
    }

    if (orientation === 'landscape') {
        [width, height] = [height, width];
    }

    return { width, height };
}

function loadImage(url) {
    return new Promise((resolve, reject) => {
        const img = new Image();
        img.onload = () => resolve(img);
        img.onerror = () => reject(new Error('Error al cargar la imagen'));
        img.src = url;
    });
}

function generatePreview() {
    if (imageUpload.files.length === 0) {
        errorMessage.style.display = 'block';
        return;
    }

    errorMessage.style.display = 'none';
    preview.innerHTML = '';
    pages = [];

    // Verificar si se especifica un tamaño de imagen
    const imageWidth = parseInt(imageWidthInput.value) * 37.795; // Convertir cm a px (1cm ≈ 37.795px)
    const imageHeight = parseInt(imageHeightInput.value) * 37.795;
    const useCustomSize = useCustomSizeCheckbox.checked;

    const files = imageUpload.files;
    const { width: pageWidth, height: pageHeight } = getPaperDimensions();
    let imagesPerRow, imagesPerColumn, imagesPerPage, gridSize;

    if (useCustomSize) {
        imagesPerRow = Math.floor(pageWidth / imageWidth);
        imagesPerColumn = Math.floor(pageHeight / imageHeight);
        imagesPerPage = imagesPerRow * imagesPerColumn;
    } else {
        imagesPerPage = parseInt(imagesPerPageSelect.value);
        gridSize = Math.ceil(Math.sqrt(imagesPerPage)); // Calcula el tamaño de la cuadrícula
    }

    let currentPage;
    let imageCount = 0;

    const imagePromises = Array.from(files).map(file => loadImage(URL.createObjectURL(file)));

    Promise.all(imagePromises).then(images => {
        images.forEach(img => {
            if (imageCount % imagesPerPage === 0) {
                if (currentPage) {
                    pages.push(currentPage);
                }
                currentPage = document.createElement('div');
                currentPage.className = 'page';
                currentPage.style.width = `${pageWidth}px`;
                currentPage.style.height = `${pageHeight}px`;
                if (useCustomSize) {
                    currentPage.style.gridTemplateColumns = `repeat(${imagesPerRow}, ${imageWidth}px)`;
                    currentPage.style.gridTemplateRows = `repeat(${imagesPerColumn}, ${imageHeight}px)`;
                } else {
                    currentPage.style.gridTemplateColumns = `repeat(${gridSize}, 1fr)`;
                    currentPage.style.gridTemplateRows = `repeat(${Math.ceil(imagesPerPage / gridSize)}, 1fr)`;
                }
            }

            const imgContainer = document.createElement('div');
            imgContainer.className = 'preview-image';
            if (useCustomSize) {
                imgContainer.style.width = `${imageWidth}px`;
                imgContainer.style.height = `${imageHeight}px`;
            }

            if (fillImageCheckbox.checked || stretchImageCheckbox.checked) {
                imgContainer.style.overflow = 'hidden';
            }

            const clonedImg = img.cloneNode();
            if (stretchImageCheckbox.checked) {
                clonedImg.style.width = '100%';
                clonedImg.style.height = '100%';
                clonedImg.style.objectFit = 'fill';
            } else {
                const aspectRatio = clonedImg.width / clonedImg.height;
                if (aspectRatio > 1) {
                    clonedImg.style.width = '100%';
                    clonedImg.style.height = 'auto';
                } else {
                    clonedImg.style.width = 'auto';
                    clonedImg.style.height = '100%';
                }
                if (fillImageCheckbox.checked) {
                    clonedImg.style.objectFit = 'cover';
                } else {
                    clonedImg.style.objectFit = 'contain';
                }

                if ((clonedImg.width > clonedImg.height && pageWidth / gridSize < pageHeight / gridSize) ||
                    (clonedImg.width < clonedImg.height && pageWidth / gridSize > pageHeight / gridSize)) {
                    clonedImg.style.transform = 'rotate(90deg)';
                    clonedImg.style.maxWidth = 'none';
                    clonedImg.style.maxHeight = 'none';
                    clonedImg.style.width = 'auto';
                    clonedImg.style.height = '100%';
                }
            }

            imgContainer.appendChild(clonedImg);
            currentPage.appendChild(imgContainer);
            imageCount++;
        });

        if (currentPage) {
            pages.push(currentPage);
        }

        totalPages = pages.length;
        showPage(0);
    }).catch(error => {
        console.error('Error al cargar las imágenes:', error);
    });
}

function showPage(index) {
    preview.innerHTML = '';
    preview.appendChild(pages[index]);

    currentPageIndex = index;

    document.getElementById('prevPage').disabled = currentPageIndex === 0;
    document.getElementById('nextPage').disabled = currentPageIndex === totalPages - 1;
}

function changePage(direction) {
    showPage(currentPageIndex + direction);
}

function printImages() {
    if (preview.innerHTML.trim() === '') {
        errorMessage.style.display = 'block';
        return;
    }

    errorMessage.style.display = 'none';
    const printWindow = window.open('', '_blank');
    printWindow.document.write('<html><head><title>Imprimir Imágenes</title>');
    printWindow.document.write('<style>');
    printWindow.document.write('body { margin: 0; }');
    printWindow.document.write('.page { width: 100%; height: 100%; display: grid; grid-template-columns: repeat(auto-fit, minmax(0, 1fr)); grid-template-rows: repeat(auto-fit, minmax(0, 1fr)); gap: 5px; }');
    printWindow.document.write('.preview-image { border: 1px solid #ccc; display: flex; justify-content: center; align-items: center; overflow: hidden; }');
    printWindow.document.write('.preview-image img { width: 100%; height: 100%; object-fit: fill; }');
    printWindow.document.write('</style></head><body>');
    pages.forEach(page => printWindow.document.write(page.outerHTML));
    printWindow.document.write('</body></html>');
    printWindow.document.close();
    printWindow.print();
}
</script>
