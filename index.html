<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>카카오 지도 API 예제</title>
    <style>
        #map {
            width: 100%;
            height: 400px;
        }
    </style>
</head>
<body>
    <h1>카카오 지도 API 예제</h1>
    <label for="start">출발 지점 좌표:</label>
    <input type="text" id="start" placeholder="출발 지점 좌표를 입력하세요">
    <br>
    <label for="end">도착 지점 좌표:</label>
    <input type="text" id="end" placeholder="도착 지점 좌표를 입력하세요">
    <br>
    <button onclick="findRoute()">최단 경로 찾기</button>
    <div id="map"></div>

    <script type="text/javascript" src="https://dapi.kakao.com/v2/maps/sdk.js?appkey=c396eec2d60f543b080e300a54e1edf7"></script>
    <script>
        var map;
        var startMarker;
        var endMarker;

        function initMap() {
            map = new kakao.maps.Map(document.getElementById('map'), {
                center: new kakao.maps.LatLng(37.5665, 126.9780), // 서울의 좌표로 초기화
                level: 10
            });
        }

        function findRoute() {
            var startInput = document.getElementById('start');
            var endInput = document.getElementById('end');
            var startCoord = startInput.value;
            var endCoord = endInput.value;

            // 입력값 검증
            if (!startCoord || !endCoord) {
                alert('출발 지점과 도착 지점을 입력하세요.');
                return;
            }

            // 출발 지점과 도착 지점 좌표로 마커 생성
            var startLatLng = new kakao.maps.LatLng(startCoord.split(',')[0], startCoord.split(',')[1]);
            var endLatLng = new kakao.maps.LatLng(endCoord.split(',')[0], endCoord.split(',')[1]);

            if (startMarker) {
                startMarker.setMap(null);
            }
            if (endMarker) {
                endMarker.setMap(null);
            }

            startMarker = new kakao.maps.Marker({
                position: startLatLng
            });
            endMarker = new kakao.maps.Marker({
                position: endLatLng
            });

            startMarker.setMap(map);
            endMarker.setMap(map);

            // 출발 지점과 도착 지점을 연결하는 최단 경로 표시
            var route = new kakao.maps.services.Places();
            route.viaPoints = [startLatLng, endLatLng];

            route.route([
                {
                    title: '출발 지점',
                    latlng: startLatLng
                },
                {
                    title: '도착 지점',
                    latlng: endLatLng
                }
            ], function(result, status) {
                if (status === kakao.maps.services.Status.OK) {
                    var path = result[0].path;
                    var distance = result[0].distance;

                    var polyline = new kakao.maps.Polyline({
                        path: path,
                        strokeWeight: 4,
                        strokeColor: '#FF0000',
                        strokeOpacity: 0.7,
                        strokeStyle: 'solid'
                    });

                    polyline.setMap(map);

                    alert('최단 거리: ' + distance + 'm');
                } else {
                    alert('최단 경로를 찾을 수 없습니다.');
                }
            });
        }
    </script>
    <script>
        kakao.maps.load(initMap);
    </script>
</body>
</html>
