          На GitHub создаем New repositoriy
						(например ../GitHub_HW_2)
						делаем в Git Bash git clone https://github.com/KlimentsiLiakhavets/GitHub_HW_2.git
						cd GitHub_HW_2
```
1. На локальном репозитории сделать ветки для:
- Postman					git branch postman
- Jmeter					git branch jmeter
- CheckLists					git branch checklists
- Bag Reports					git branch bag_reports
- SQL						git branch SQL
- Charles					git branch charles
- Mobile testing				git branch mobile_testing

2. Запушить все ветки на внешний репозиторий	git push origin --all

3. В ветке Bag Reports сделать текстовый 	git checkout bag_reports
   документ со структурой баг репорта		touch bag_reports.txt
						vim bag_reports.txt
						i
						1. Идентификационный номер	(ID)
						2. Краткое описание бага	(Summary)
						3. Название проекта		(Project)
						4. Точная версия ПО		(Version)
						5. Дата обнаружения		(Date detected)
						6. Серьезность бага		(Severity)
						7. Приоритет			(Priority)
						8. Статус			(Status)
						9. Автор			(Detected by)
						10. Исполнитель			(Assigned to)
						11. Шаги воспроизведения	(Steps to reproduce)
						12. Фактический результат	(Actual result)
						13. Ожидаемый результат		(Expected result)
						14. Дополнения			(Additional information)
						Esc
						:wq

4. Запушить структуру багрепорта на внешний 	git add bag_reports.txt
   репозиторий					git commit -m "structure"
						git push origin bag_reports

5. Вмержить ветку Bag Reports в Main		git checkout main
						git merge bag_reports

6. Запушить main на внешний репозиторий.	git push origin main

7. В ветке CheckLists набросать структуру 	git checkout checklists
   чек листа.					touch list.txt
						vim list.txt
						i
						1. Номер
						2. Проверка, т.е. действия тестировщика
						3. Результат
						4. Комментарий
						Esc
						:wq
						git add list.txt
						git commit -m "structure"

8. Запушить структуру на внешний репозиторий	git push origin checklists

9. На внешнем репозитории сделать 		в GitHub (ветка checklist) нажимаем Pull Request
   Pull Request ветки CheckLists в main		checklist -> main  сохраняем

10. Синхронизировать Внешнюю и Локальную 	в gitbash команда git pull
    ветки Main
