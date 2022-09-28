# Projekt końcowy - Opóźnienie lotu



## Getting started

To make it easy for you to get started with GitLab, here's a list of recommended next steps.

Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!

## Add your files

- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:

```
cd existing_repo
git remote add origin https://gitlab.com/m4691/projekt-koncowy-opoznienie-lotu.git
git branch -M main
git push -uf origin main
```

## Integrate with your tools

- [ ] [Set up project integrations](https://gitlab.com/m4691/projekt-koncowy-opoznienie-lotu/-/settings/integrations)

## Collaborate with your team

- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)
- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)
- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)
- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)
- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)

## Test and Deploy

Use the built-in continuous integration in GitLab.

- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)
- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)
- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)
- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)
- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)

***

## Name
Prognozowanie opóźnień lotów

## Description
Przy dzisijszym tempie życia ludzie oczekują działania według znanego harmonogramu. Sytuacje odbiegające od przewidzianego harmonogramem czasu powodują koszty. Dlatego tak ważne jest wcześniejsze przewidywanie opóźnień.
Nasz projekt opiera się na datasecie z portalu kaggle (https://www.kaggle.com/usdot/flight-delays?select=flights.csv). 
Ze względu na dużą ilość danych modele zostały wytrenowane na danych z jednego miesiąca. Metryki klasyfikacji opóźnień zostały wyliczone dla wybranych modeli: regresji logistycznej, najbliższych sąsiadów oraz drzewa decyzyjnego. Metryki dla wszystkich modeli wyszły lepsze niż dla modelu baseline'owego, co jest zgodne z oczekiwaniami. Najlepszym modelem w przypadku zdefiniowanego problemu okazał się model k najbliższych sąsiadów, ponieważ jego czułość odnotowała najwyższy wynik spośród wytrenowanych modeli. Czułość w tym przypadku jest kluczowym wskaźnikiem, ponieważ ważna jest ilość wykrytych opóźnień spośród wszystkich lotów. Im więcej wykrytych poprawnie opóźnień lotów, tym mniej nieprzyjemnego zaskoczenia dla człowieka. 


## Installation
W celu skorzystania z projektu należy pobrać notatnik i najlepiej otworzyć go za pomocą Google Collab. Projekt zawiera dane z platformy kaggle. Należy zalogować się na platformie i pobrać odpowiedni token API w formacie json. Ścieżka do tokena: Your Profile -> Account -> API -> Crete New API Token. Pobrany plik należy załączyć do środowiska w Google Colab.


## Support
Pomocą w zrozumieniu projektu służą właściciele projektu.

## Authors and acknowledgment
Projekt powstał dzięki uczestnictwu w kursie Data Science od SDA.

## Project status
Projekt stanowi podstawową wersję predykcji opónień lotów.
Pomysłem na dalsze rozwijanie projektu może być prognozowanie opóźnień lotów na podstawie danych pogodowych. 
