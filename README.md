# DataStore
lib per salvare i dati in modo molto veloce
    
1 aggiungere la libreria  nel maven 
settings.gradle
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        mavenCentral()
        mavenCentral() // Warning: this repository is going to shut down soon
        maven { url 'https://jitpack.io'
        }
    }
}
2 maven
implementation 'com.github.angiof:DataStore:1.0.0'
3 basta aggiungere i dati usando il costrutto saveParam
p.saveParam(requireActivity(), "id", entityPassword.id)
e ricervergli cosi 
p.getParam(requireActivity(), "p").toString()
