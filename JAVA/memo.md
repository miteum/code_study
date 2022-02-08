# 메모장 실습





note 

```
package com.codelatte.memo.usecase;

import com.codelatte.memo.note.NotePad;

import java.util.Scanner;

public class NoteService {

    private final NotePad notePad;

    public NoteService() {
        this.notePad = new NotePad();
    }

    public void run() {
        // TODO : 메모장 프로그램의 실행
        while (true) {
            Scanner scanner = new Scanner(System.in);

            System.out.println("안녕하세요. 메모장입니다");
            System.out.println("1.메모 전체보기 2.메모보기 3.메모작성 4.메모수정 5.메모삭제 6.종료");
            System.out.println("번호를 입력해주세요");

            int selectedNumber = scanner.nextInt();

            if (1 == selectedNumber) {
                // TODO : 메모 전체보기 처리
                notePad.printAllNotes();
            } else if (2 == selectedNumber) {
                // TODO : 메모 상세보기 처리
                notePad.printNote();
            } else if (3 == selectedNumber) {
                // TODO : 메모 작성하기 처리
                notePad.addNote();
            } else if (4 == selectedNumber) {
                // TODO : 메모 수정하기 처리
                notePad.updateNote();
            } else if (5 == selectedNumber) {
                //  TODO: 메모 삭제하기 처리
                 notePad.deletNote();
            } else if (6 == selectedNumber) {
                break;
            } else {
                System.out.println("");
                System.out.println("번호를 다시입력해주세요");
                System.out.println("");
            }
        }
    }


}
```





메모 작성

```
   public void addNote() {
        System.out.println("");
        if (NOTE_SIZE == this.noteLength) {
            System.out.println("메모가 꽉찼습니다");
            System.out.println("");
            return;
        }

        Scanner scanner = new Scanner(System.in);
        System.out.println("제목을 작성해주세요");
        String title = scanner.nextLine();

        System.out.println("본문을 작성해주세요");
        String content = scanner.nextLine();

        noteEntities[this.noteLength++] = NoteEntity.newInstance(title, content);

        System.out.println("메모가 작성되었습니다");
        System.out.println("");
    }
```

