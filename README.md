<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Respaldamos Colombia - Proyección de Inversión</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
            height: 350px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
        }
        .flowchart-step {
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 1rem;
            border-radius: 0.5rem;
            box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
            min-height: 120px;
        }
        .flowchart-arrow {
            font-size: 2rem;
            font-weight: bold;
            color: #2C66AB;
            margin: 0 1rem;
            transform: rotate(90deg);
        }
         @media (min-width: 768px) {
            .flowchart-arrow {
                 transform: rotate(0deg);
            }
        }
    </style>
</head>
<body class="bg-gray-100 text-gray-800">
<!-- Neither Mermaid JS nor SVG were used in this output. -->
<!-- Plan de la infografía:
  - Portada: Título, subtítulo y logo de la firma.
  - Problema & Solución: Exponer la necesidad del mercado y nuestra propuesta de valor en tarjetas separadas.
  - Modelo de Adquisición: Detallar la estrategia de marketing digital.
  - Escenarios de Inversión: Visualizar los 3 escenarios con un gráfico de barras.
  - Plan de Arranque: Representar el flujo de trabajo semanal con un diagrama simple.
  - Proyección a 6 Meses: Resaltar el retorno de la inversión con un gráfico comparativo.
  - Cierre: Mensaje final y llamado a la acción.
  - Visualizaciones:
    - Escenarios: Se utilizará un gráfico de barras (Bar Chart) con Chart.js para comparar la inversión, los leads, los clientes y los ingresos en los 3 escenarios, lo cual es ideal para comparar múltiples variables.
    - Proyección: Se usará un gráfico de barras horizontal (Horizontal Bar Chart) con Chart.js para comparar la inversión total vs. los ingresos proyectados en 6 meses para los 2 escenarios clave, lo que lo hace muy claro para la lectura.
    - Plan de Arranque: Se usará un diagrama de flujo simple de HTML/CSS con Flexbox y estilos de Tailwind para organizar visualmente los pasos.
-->
    <header class="bg-[#0A2342] text-white p-8 text-center">
        <h1 class="text-4xl md:text-5xl font-bold mb-2">Respaldamos Colombia</h1>
        <h2 class="text-xl md:text-2xl font-light">Proyección de Inversión en Ads – Ronda Family & Friends</h2>
        <p class="mt-2 text-lg text-[#84A9C0]">Septiembre 2025</p>
    </header>

    <main class="container mx-auto p-4 md:p-8">

        <section id="problema-solucion" class="mb-12">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <h3 class="text-2xl font-bold text-[#0A2342] mb-4">El Problema: Una Carga Financiera para Millones</h3>
                    <p class="mb-4">Muchos colombianos enfrentan una alta carga financiera debido a sus créditos hipotecarios, lo que compromete su estabilidad económica y limita sus oportunidades.</p>
                    <p>Adicionalmente, existe un profundo desconocimiento sobre las herramientas legales disponibles que podrían aliviar significativamente estas deudas y proteger su patrimonio.</p>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <h3 class="text-2xl font-bold text-[#0A2342] mb-4">Nuestra Solución: Experiencia Legal y Financiera</h3>
                    <p class="mb-4">Ofrecemos un servicio legal especializado en la reducción de créditos hipotecarios. Analizamos cada caso para aplicar las estrategias legales que permitan optimizar la deuda del cliente.</p>
                    <div class="space-y-3">
                        <p><strong class="text-[#2C66AB]">✔ Reducción de la Deuda:</strong> Disminuimos el monto total del crédito.</p>
                        <p><strong class="text-[#2C66AB]">✔ Ahorro a Largo Plazo:</strong> Menos intereses y capital a pagar.</p>
                        <p><strong class="text-[#2C66AB]">✔ Protección del Patrimonio:</strong> Aliviamos la presión financiera sobre los activos familiares.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="adquisicion" class="bg-white p-6 rounded-lg shadow-md mb-12 text-center">
            <h3 class="text-2xl font-bold text-[#0A2342] mb-4">Modelo de Adquisición de Clientes</h3>
            <p class="max-w-3xl mx-auto">Nuestra estrategia de crecimiento se centra en un modelo de marketing digital robusto y escalable. Invertiremos en publicidad a través de plataformas clave como Facebook, Instagram y Google Ads para llegar a nuestro público objetivo de manera precisa. El enfoque no es solo generar un alto volumen de prospectos, sino captar leads altamente calificados, optimizando cada peso invertido para maximizar la tasa de conversión a clientes.</p>
        </section>

        <section id="escenarios" class="mb-12">
            <h3 class="text-3xl font-bold text-center text-[#0A2342] mb-2">Escenarios de Inversión Mensual</h3>
             <p class="text-center text-gray-600 mb-6 max-w-3xl mx-auto">Presentamos tres niveles de inversión para escalar la adquisición de clientes. Cada escenario muestra el potencial de crecimiento basado en la inversión mensual en publicidad, detallando los resultados máximos esperados en leads, clientes e ingresos.</p>
            <div class="bg-white p-6 rounded-lg shadow-md">
                <div class="chart-container">
                    <canvas id="investmentScenariosChart"></canvas>
                </div>
            </div>
        </section>
        
        <section id="plan-arranque" class="mb-12">
             <h3 class="text-3xl font-bold text-center text-[#0A2342] mb-2">Plan de Arranque Acelerado (Primer Mes)</h3>
             <p class="text-center text-gray-600 mb-6 max-w-3xl mx-auto">Nuestro plan de arranque está diseñado para optimizar la inversión desde el primer día, pasando de una fase de testeo a un flujo constante de clientes en solo tres semanas.</p>
             <div class="bg-white p-6 rounded-lg shadow-md">
                 <div class="flex flex-col md:flex-row items-center justify-center">
                    <div class="flowchart-step bg-[#E0E8F0] text-[#0A2342] w-full md:w-1/4">
                        <div>
                            <h4 class="font-bold text-lg">Semana 1</h4>
                            <p>Testeo de mensajes y segmentación con una inversión de 100k.</p>
                        </div>
                    </div>
                    <div class="flowchart-arrow">➔</div>
                    <div class="flowchart-step bg-[#84A9C0] text-white w-full md:w-1/4">
                         <div>
                            <h4 class="font-bold text-lg">Semana 2</h4>
                            <p>Optimización basada en datos, duplicando la inversión a 200k.</p>
                        </div>
                    </div>
                     <div class="flowchart-arrow">➔</div>
                    <div class="flowchart-step bg-[#2C66AB] text-white w-full md:w-1/4">
                         <div>
                            <h4 class="font-bold text-lg">Semana 3 en adelante</h4>
                            <p>Escalamiento a 300k/semana para un flujo constante de leads.</p>
                        </div>
                    </div>
                </div>
             </div>
        </section>

        <section id="proyeccion" class="mb-12">
            <h3 class="text-3xl font-bold text-center text-[#0A2342] mb-2">Proyección de Retorno a 6 Meses</h3>
            <p class="text-center text-gray-600 mb-6 max-w-3xl mx-auto">La inversión total durante seis meses se traduce en un potencial de ingresos significativo, demostrando la rentabilidad del modelo tanto en el escenario mínimo como en el ideal.</p>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="bg-white p-6 rounded-lg shadow-md text-center">
                    <h4 class="text-xl font-bold text-[#0A2342]">Inversión Mínima</h4>
                    <p class="text-4xl font-bold text-[#2C66AB] my-4">6M COP</p>
                    <p class="text-gray-700">Genera hasta</p>
                    <p class="text-5xl font-bold text-green-600 mt-2">80M COP</p>
                    <p class="text-gray-700">en ingresos</p>
                </div>
                 <div class="bg-white p-6 rounded-lg shadow-md text-center">
                    <h4 class="text-xl font-bold text-[#0A2342]">Inversión Ideal</h4>
                    <p class="text-4xl font-bold text-[#2C66AB] my-4">18M COP</p>
                    <p class="text-gray-700">Genera más de</p>
                    <p class="text-5xl font-bold text-green-600 mt-2">200M COP</p>
                    <p class="text-gray-700">en ingresos</p>
                </div>
            </div>
             <div class="bg-white p-6 rounded-lg shadow-md mt-8">
                <div class="chart-container" style="height:300px; max-height:350px;">
                    <canvas id="projectionChart"></canvas>
                </div>
            </div>
        </section>

        <section id="gemini-feature" class="mb-12 bg-white p-6 rounded-lg shadow-md text-center">
            <h3 class="text-2xl font-bold text-[#0A2342] mb-4">✨ Analiza tu Inversión Personalizada ✨</h3>
            <p class="max-w-3xl mx-auto text-gray-600 mb-4">Ingresa el monto que te gustaría invertir mensualmente y nuestra inteligencia artificial te dará una proyección personalizada de los resultados.</p>
            <div class="flex flex-col md:flex-row items-center justify-center space-y-4 md:space-y-0 md:space-x-4 mb-6">
                <input type="number" id="investmentInput" class="w-full md:w-1/2 p-3 border border-gray-300 rounded-lg focus:outline-none focus:border-[#2C66AB]" placeholder="Monto mensual en COP (ej. 500000)">
                <button id="analyzeButton" class="w-full md:w-1/2 bg-[#2C66AB] text-white p-3 rounded-lg font-semibold hover:bg-[#1E4D8A] transition-colors duration-200">
                    Generar Proyección
                </button>
            </div>
            <div id="resultsContainer" class="mt-4 text-left">
                <p id="loadingIndicator" class="text-center text-gray-500 hidden">Generando análisis, por favor espera...</p>
            </div>
        </section>

        <footer class="bg-[#0A2342] text-white p-8 text-center rounded-lg shadow-md">
            <h3 class="text-2xl md:text-3xl font-bold mb-4">Únete a Respaldamos Colombia</h3>
            <p class="max-w-3xl mx-auto text-lg mb-4 text-[#D9D9D9]">Protegemos el patrimonio de las familias colombianas, mientras generamos rentabilidad para nuestros aliados.</p>
            <p class="text-xl font-semibold">Invierte en un negocio con propósito y un crecimiento proyectado.</p>
        </footer>

    </main>

    <script>
        document.addEventListener('DOMContentLoaded', function () {
            const tooltipTitleCallback = {
                plugins: {
                    tooltip: {
                        callbacks: {
                            title: function(tooltipItems) {
                                const item = tooltipItems[0];
                                let label = item.chart.data.labels[item.dataIndex];
                                if (Array.isArray(label)) {
                                    return label.join(' ');
                                } else {
                                    return label;
                                }
                            }
                        }
                    }
                }
            };
            
            const brilliantBlues = {
                dark: '#0A2342',
                medium: '#2C66AB',
                light: '#84A9C0',
                gray: '#D9D9D9'
            };

            const investmentCtx = document.getElementById('investmentScenariosChart').getContext('2d');
            new Chart(investmentCtx, {
                type: 'bar',
                data: {
                    labels: ['Mínimo (aprendizaje)', 'Razonable (funcionamiento)', 'Ideal (aceleración)'],
                    datasets: [
                        {
                            label: 'Inversión Mensual (COP)',
                            data: [500000, 1200000, 3000000],
                            backgroundColor: brilliantBlues.light,
                            yAxisID: 'y',
                            order: 2,
                        },
                        {
                            label: 'Ingresos Estimados (COP)',
                            data: [4000000, 12000000, 40000000],
                            backgroundColor: brilliantBlues.medium,
                            yAxisID: 'y',
                            order: 2,
                        },
                        {
                            label: 'Leads Estimados',
                            data: [20, 60, 150],
                            backgroundColor: 'rgba(217, 217, 217, 0.8)',
                            yAxisID: 'y1',
                            order: 1,
                        },
                        {
                            label: 'Clientes Estimados',
                            data: [1, 3, 10],
                            backgroundColor: brilliantBlues.dark,
                            yAxisID: 'y1',
                            order: 1,
                        }
                    ]
                },
                options: {
                    ...tooltipTitleCallback,
                    maintainAspectRatio: false,
                    responsive: true,
                    scales: {
                        x: {
                            stacked: true,
                             ticks: {
                                color: brilliantBlues.dark,
                                font: {
                                    weight: '600'
                                }
                            }
                        },
                        y: {
                            type: 'linear',
                            display: true,
                            position: 'left',
                            title: {
                                display: true,
                                text: 'Monto (COP)',
                                color: brilliantBlues.medium
                            },
                             ticks: {
                                callback: function(value, index, values) {
                                    return (value / 1000000) + 'M';
                                }
                            }
                        },
                        y1: {
                            type: 'linear',
                            display: true,
                            position: 'right',
                            title: {
                                display: true,
                                text: 'Cantidad (Leads/Clientes)',
                                color: brilliantBlues.dark
                            },
                            grid: {
                                drawOnChartArea: false,
                            }
                        }
                    },
                    plugins: {
                        ...tooltipTitleCallback.plugins,
                        legend: {
                           position: 'top',
                        },
                    }
                }
            });

            const projectionCtx = document.getElementById('projectionChart').getContext('2d');
            new Chart(projectionCtx, {
                type: 'bar',
                data: {
                    labels: ['Inversión Mínima', 'Inversión Ideal'],
                    datasets: [{
                        label: 'Inversión Total a 6 Meses (COP)',
                        data: [6000000, 18000000],
                        backgroundColor: brilliantBlues.medium,
                        borderColor: brilliantBlues.dark,
                        borderWidth: 1,
                        yAxisID: 'y'
                    }, {
                        label: 'Ingresos Potenciales (COP)',
                        data: [80000000, 200000000],
                        backgroundColor: 'rgba(34, 197, 94, 0.7)',
                        borderColor: 'rgba(22, 163, 74, 1)',
                        borderWidth: 1,
                        yAxisID: 'y'
                    }]
                },
                options: {
                    ...tooltipTitleCallback,
                    maintainAspectRatio: false,
                    responsive: true,
                    indexAxis: 'y',
                    scales: {
                        x: {
                             title: {
                                display: true,
                                text: 'Monto (COP)',
                                color: brilliantBlues.dark
                            },
                             ticks: {
                                callback: function(value, index, values) {
                                    return (value / 1000000) + 'M';
                                }
                            }
                        },
                        y: {
                            beginAtZero: true,
                             ticks: {
                                color: brilliantBlues.dark,
                                font: {
                                    size: 14,
                                    weight: 'bold'
                                }
                            }
                        }
                    }
                }
            });

            const investmentInput = document.getElementById('investmentInput');
            const analyzeButton = document.getElementById('analyzeButton');
            const resultsContainer = document.getElementById('resultsContainer');
            const loadingIndicator = document.getElementById('loadingIndicator');

            analyzeButton.addEventListener('click', async () => {
                const investment = investmentInput.value;
                if (!investment || isNaN(investment) || investment <= 0) {
                    resultsContainer.innerHTML = '<p class="text-red-500">Por favor, ingresa un monto de inversión válido.</p>';
                    return;
                }

                loadingIndicator.classList.remove('hidden');
                resultsContainer.innerHTML = '';
                
                const userQuery = `Calcula las proyecciones de inversión en un periodo de 6 meses para la firma de abogados "Respaldamos Colombia" con una inversión mensual en marketing digital de ${investment} COP. Proporciona leads estimados, clientes estimados e ingresos estimados, junto con una explicación de por qué estos números son una buena proyección. El modelo de negocio se basa en convertir leads en clientes, donde la reducción de créditos hipotecarios es el servicio principal. Usa una base de conversión de 0.5% a 2% de leads a clientes y un ingreso promedio por cliente de 4M COP. Los ingresos de leads y clientes deben ser aproximaciones.`;
                const systemPrompt = `Eres un analista financiero experto en el modelo de negocio de la firma de abogados "Respaldamos Colombia", especializada en la reducción de créditos hipotecarios. Tu tarea es generar un análisis de proyección de inversión basado en un monto mensual dado. Sé conciso y profesional.`;

                const payload = {
                    contents: [{ parts: [{ text: userQuery }] }],
                    systemInstruction: { parts: [{ text: systemPrompt }] },
                    generationConfig: {
                        responseMimeType: "application/json",
                        responseSchema: {
                            type: "OBJECT",
                            properties: {
                                "inversionMensual": { "type": "NUMBER" },
                                "inversionTotal": { "type": "NUMBER" },
                                "leadsEstimados": { "type": "STRING" },
                                "clientesEstimados": { "type": "STRING" },
                                "ingresosEstimados": { "type": "STRING" },
                                "analisis": { "type": "STRING" }
                            }
                        }
                    }
                };

                const apiKey = "";
                const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-05-20:generateContent?key=${apiKey}`;

                try {
                    const response = await fetch(apiUrl, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });
                    
                    const result = await response.json();
                    const jsonResponse = JSON.parse(result.candidates[0].content.parts[0].text);

                    resultsContainer.innerHTML = `
                        <div class="bg-[#F0F7FF] p-6 rounded-lg shadow-inner">
                            <h4 class="text-xl font-bold text-[#0A2342] mb-2">Proyección Generada por IA:</h4>
                            <p class="mb-2"><strong>Inversión Mensual:</strong> ${jsonResponse.inversionMensual.toLocaleString('es-CO', { style: 'currency', currency: 'COP' })}</p>
                            <p class="mb-2"><strong>Inversión Total (6 Meses):</strong> ${jsonResponse.inversionTotal.toLocaleString('es-CO', { style: 'currency', currency: 'COP' })}</p>
                            <p class="mb-2"><strong>Leads Estimados:</strong> ${jsonResponse.leadsEstimados}</p>
                            <p class="mb-2"><strong>Clientes Estimados:</strong> ${jsonResponse.clientesEstimados}</p>
                            <p class="mb-4"><strong>Ingresos Estimados (6 Meses):</strong> ${jsonResponse.ingresosEstimados}</p>
                            <div class="p-4 bg-white rounded-lg border border-[#D9D9D9]">
                                <h5 class="font-semibold text-lg text-[#2C66AB] mb-1">Análisis:</h5>
                                <p class="text-gray-700">${jsonResponse.analisis}</p>
                            </div>
                        </div>
                    `;

                } catch (error) {
                    console.error('Error al generar la proyección:', error);
                    resultsContainer.innerHTML = `<p class="text-red-500">Ocurrió un error al generar la proyección. Por favor, inténtalo de nuevo.</p>`;
                } finally {
                    loadingIndicator.classList.add('hidden');
                }
            });
        });
    </script>
</body>
</html>
