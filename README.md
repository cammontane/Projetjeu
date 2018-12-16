<!doctype html>
<html>

<head>
    <meta charset="utf-8">
    <title>Jeu</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO"
        crossorigin="anonymous">
    <link rel="stylesheet" href="bootstrap.css">
    <link rel="stylesheet" href="jeu.css">
    <script src="https://code.jquery.com/jquery-1.12.4.js"></script>
    <script src="https://code.jquery.com/ui/1.12.1/jquery-ui.js"></script>
    <link href="https://fonts.googleapis.com/css?family=Bungee+Inline|Monoton" rel="stylesheet">
    <script src="jeu.js"></script>
    <script src="bootstrap.js"></script>

</head>

<body>
    <div class="container-fluid">
        <div id="presentEquipe" class="row justify-content-center">
            <div class="col-6">
                <ul id="selectionDom" class="selection">
                    <li class="listEquipe">Amiens</li>
                    <li class="listEquipe">Angers</li>
                    <li class="listEquipe">Bordeaux</li>
                    <li class="listEquipe">Caen</li>
                    <li class="listEquipe">Dijon</li>
                    <li class="listEquipe">Guingamp</li>
                    <li class="listEquipe">Lille</li>
                    <li class="listEquipe">Lyon</li>
                    <li class="listEquipe">Marseille</li>
                    <li class="listEquipe">Monaco</li>
                    <li class="listEquipe">Montpellier</li>
                    <li class="listEquipe">Nantes</li>
                    <li class="listEquipe">Nice</li>
                    <li class="listEquipe">Nimes</li>
                    <li class="listEquipe">Paris SG</li>
                    <li class="listEquipe">Reims</li>
                    <li class="listEquipe">Rennes</li>
                    <li class="listEquipe">Saint-Etienne</li>
                    <li class="listEquipe">Strasbourg</li>
                    <li class="listEquipe">Toulouse</li>
                </ul>
            </div>
            <div class="col-6" id="colonne3">
                <ul id="selectionExt" class="selection">
                    <li class="listEquipe">Amiens</li>
                    <li class="listEquipe">Angers</li>
                    <li class="listEquipe">Bordeaux</li>
                    <li class="listEquipe">Caen</li>
                    <li class="listEquipe">Dijon</li>
                    <li class="listEquipe">Guingamp</li>
                    <li class="listEquipe">Lille</li>
                    <li class="listEquipe">Lyon</li>
                    <li class="listEquipe">Marseille</li>
                    <li class="listEquipe">Monaco</li>
                    <li class="listEquipe">Montpellier</li>
                    <li class="listEquipe">Nantes</li>
                    <li class="listEquipe">Nice</li>
                    <li class="listEquipe">Nîmes</li>
                    <li class="listEquipe">Paris SG</li>
                    <li class="listEquipe">Reims</li>
                    <li class="listEquipe">Rennes</li>
                    <li class="listEquipe">Saint-Etienne</li>
                    <li class="listEquipe">Strasbourg</li>
                    <li class="listEquipe">Toulouse</li>
                </ul>
            </div>

        </div>

        <div class="choix">
            <button type="button" class="choix" onclick="choix()" data-toggle="modal" data-target="#modelId">
                Match
            </button>
        </div>

        <div class="modal fade" id="modelId" tabindex="-1" role="dialog" aria-labelledby="modelTitleId" aria-hidden="true">
            <div class="modal-body">
                <div class="container-fluid">
                    <div class="row row1">
                        <div class="col-6"><input type="text" id="dom" value="" class="equipe"></div>
                        <div class="col-6"><input type="text" id="ext" value="" class="equipe"></div>
                    </div>
                    <div class="row rowscore">
                        <div class="col-6" id="score1">0</div>
                        <div class="col-6" id="score2">0</div>
                    </div>
                    <div class="row rowminutebut" style="height:50px">
                        <div class="col-6" id="minute1"></div>
                        <div class="col-6" id="minute2"></div>
                    </div>
                    <div class="row rowtemps" style="height:100px">
                        <div class="col" id="temps"></div>
                    </div>

                    <div class="row rowbut" style="height:50px">
                        <div class="col" id="minuteBut"></div>
                    </div>

                    <div class="row rowstats1" style="height:30px">
                        <div class="col-5 col-sm-7">Tirs : </div>
                        <div class="col-1 mr-3" id="tirs1"></div>
                        <div class="col-1" id="tirs2"></div>
                    </div>
                    <div class="row rowstats1" style="height:30px">
                        <div class="col-5 col-sm-7">Possession : </div>
                        <div class="col-1 mr-3 mr-md-4" id="possessionResult1"></div>
                        <div class="col-1" id="possessionResult2"></div>
                    </div>
                </div>
                <div class="modal-dialog" role="document">
                </div>
                <div class="modal-header">
                </div>
                <div class="modal-footer">
                    <div class="col"><button type="button" name="button" onclick=choix() class="btn btn-secondary">Nouveau
                            match</button></div>
                    <button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>

                </div>
            </div>
        </div>
    </div>
    </div>
</body>

</html>

