<?php

namespace App\Http\Controllers;

use Illuminate\Http\Request;

use Illuminate\Support\Facades\Http;

class ClintController extends Controller
{
    public function getAllData(){
        $response = HTTP::get('https://jsonplaceholder.typicode.com/posts');
        return $response->json();
    }

    public function getPostById($id){
        $response = HTTP::get('https://jsonplaceholder.typicode.com/posts'.$id);
        return $response->json();
    }

    public function addPost(){
        $response = HTTP::post('https://jsonplaceholder.typicode.com/posts',[
            'userId'=>1,
            'title'=>'New Year',
            'body' =>'New Post submited'
        ]);
        return $response->json();
    }
}
