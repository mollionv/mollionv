```cpp
// Compte GitHub secondaire, dédié à mes études (projets IUT, TP, cours).
 
#include <string>
#include <vector>
#include <map>
 
class Virgile {
public:
    std::string name     = "Virgile Mollion";
    std::string location = "Grenoble, France";
 
    std::map<std::string, std::string> education = {
        {"current", "BUT Informatique - IUT2 Grenoble (2e année)"},
        {"next",    "Échange universitaire - ÉTS Montréal (2027 - 2028)"}
    };
 
    std::vector<std::string> interests = {"cybersécurité", "recherche", "machine learning"};
    std::string lookingFor = "Stage de mi-avril à juin 2027";
 
    std::vector<std::string> experience() const {
        return {
            "Stage - Laboratoire ITODYS (CNRS) : modèle de machine learning",
            "Stage - Laboratoire ITODYS (CNRS) : analyse de données en Python"
        };
    }
 
    std::map<std::string, std::vector<std::string>> stack() const {
        return {
            {"languages", {"Python", "Go", "C", "C++", "Java", "PHP", "R"}},
            {"web_data",  {"HTML/CSS", "SQL", "PostgreSQL"}},
            {"systems",   {"Linux", "Docker", "Cloudflare"}}
        };
    }
 
    std::map<std::string, std::string> contact() const {
        return {
            {"portfolio", "https://virgile.tech"},
            {"email",     "virgile.mollion@etu.univ-grenoble-alpes.fr"}
        };
    }
};
 
int main() {
    Virgile me;
    return 0;
}
```
