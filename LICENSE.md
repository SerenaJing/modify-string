
          function Order(str) {
            var arr = [];
            var temp;
            arr = str.split('');
            if(arr.length == 0) return '';
            var length = arr.length;
            var i,j;
            for(i=0;i<length;i++) {
              if(arr[i]>='A' && arr[i]<='Z') {
                temp = arr[i];
                arr.splice(i, 1);
                length--;
                i--;
                console.log(i);
                arr.push(temp);
                console.log(arr.join(''));
              }
            }
            console.log(arr.join(''));
          }

        var str = 'aabBDaCsCUaaaH';
        var result = Order(str);
