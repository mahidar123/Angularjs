# Angularjs
<html>
  <head> <title> My Angular framework </title>
    <script src="angular.min.js"> </script>
  </head>
  <body>
    <script src="http://ajax.google.apis.com/ajax/libs/angularjs/1.4.8/angular.min.js"> </script>
    <div ng-app="Mahi" ng-controller="Mahictrl">
      <p> Type country name: <input type="text" ng-model="test"> </p>
      <ol>
        <li ng-repeat="x in countryNames | filter:test">
          {{x}}
        </li>
      </ol>
    </div>
    <script>
      angular.module('Mahi',[]).controller('Mahictrl',function($scope){
      $scope.countryNames=['Afghanishan','India','Australia','Andorra','Bangladesh','Cambodia','China','Denmark','Egypt','USSR']});
    </script>
  </body>
</html>
  
