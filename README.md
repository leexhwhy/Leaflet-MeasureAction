# Leaflet-MeasureAction
based on ToolbarAction

![image](https://github.com/shitao1988/Leaflet-MeasureAction/raw/master/1.png)

         var measureline = L.ComputeDist.extend({
                options: {
                    toolbarIcon: {
                        html: '<div class="toolbar_measuerline" title="测距"></div>',
                        tooltip: '测距'
                    }
                }
            });
              var measurearea = L.ComputeArea.extend({
                options: {
                    toolbarIcon: {
                        html: '<div class="toolbar_measuerarea" title="测面"></div>',
                        tooltip: '测面'
                    }
                }
            });
          new L.Toolbar.Control({
                position: 'topleft',
                actions: [measureline, measurearea],
            }).addTo(map);
