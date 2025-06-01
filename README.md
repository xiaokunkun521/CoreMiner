<script>
        document.addEventListener('DOMContentLoaded', function() {
            const fontSizeSlider = document.getElementById('fontSize');
            const fontSizeValue = document.getElementById('fontSizeValue');
            const updateBtn = document.getElementById('updateBtn');
            const gradientPreview = document.getElementById('gradientPreview');
            const textElement = gradientPreview.querySelector('text');
            const gradientElement = gradientPreview.querySelector('linearGradient');
            
            // 更新字体大小显示值
            fontSizeSlider.addEventListener('input', function() {
                fontSizeValue.textContent = this.value;
            });
            
            // 更新预览
            updateBtn.addEventListener('click', function() {
                const size = fontSizeSlider.value;
                const gradientType = document.getElementById('gradientType').value;
                const color1 = document.getElementById('color1').value;
                const color2 = document.getElementById('color2').value;
                
                // 更新字体大小
                textElement.setAttribute('font-size', size);
                
                // 调整SVG高度以适应新字体大小
                gradientPreview.setAttribute('height', parseInt(size) * 2 + 20);
                
                // 更新渐变方向
                if (gradientType === 'vertical') {
                    gradientElement.setAttribute('x1', '0%');
                    gradientElement.setAttribute('y1', '0%');
                    gradientElement.setAttribute('x2', '0%');
                    gradientElement.setAttribute('y2', '100%');
                } else if (gradientType === 'diagonal') {
                    gradientElement.setAttribute('x1', '0%');
                    gradientElement.setAttribute('y1', '0%');
                    gradientElement.setAttribute('x2', '100%');
                    gradientElement.setAttribute('y2', '100%');
                } else {
                    gradientElement.setAttribute('x1', '0%');
                    gradientElement.setAttribute('y1', '0%');
                    gradientElement.setAttribute('x2', '100%');
                    gradientElement.setAttribute('y2', '0%');
                }
                
                // 更新颜色
                const stops = gradientElement.querySelectorAll('stop');
                stops[0].setAttribute('stop-color', color1);
                stops[1].setAttribute('stop-color', color2);
            });
        });
    </script>

__一个专注于头矿币种的挖矿软件__

支持多卡挖矿

支持nvidia/AMD/intel的GPU挖矿

支持AMD/intel的CPU挖矿

公益、免费、无抽水。

做最好的挖矿软件！

最新版下载地址：https://github.com/xiaokunkun521/KKminer/releases/download/1.1.0.3/windows.zip

如果您有什么更好的建议或发现BUG请加TG群反馈,作者会在第一时间维护。

![1](https://github.com/user-attachments/assets/461afbf3-178f-40af-af9c-765209895539)

![2](https://github.com/user-attachments/assets/580bf959-bd32-4682-a459-11608b28c57c)

![3](https://github.com/user-attachments/assets/00d1a7b7-d736-4f28-84b6-06399433ee40)

![f2e453834305fc9b914d445937ab8408](https://github.com/user-attachments/assets/01bcfcc3-a23e-439d-bf40-0143d36dfc07)

__天行健，君子以自强不息；地势坤，君子以厚德载物__

