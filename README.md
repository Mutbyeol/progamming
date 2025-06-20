#include <stdio.h>
#include <stdlib.h>
#include <time.h>
int main() {
	srand(time(NULL));
	int a = 0;
	char c = 's';
	printf("게임을 시작하시겠습니까?\ny/n");
	scanf_s("%c", &c);
	while (1) {
		if (c == 'y') {
			a = 1;
			break;
		}

		else if (c == 'n') {
			printf("게임을 종료합니다");
			break;
		}

		else {
			printf("y 또는 n을 입력해주세요");
			continue;
		}
	}
	while (a) {
		printf("어서오세요");
	}
	return 0;
}
